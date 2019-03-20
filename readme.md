# SCSS Grid

Very simple grid for your projects.

## Mixins

- breakpoint

  ```scss
  @include breakpoint($bpMobile) {
    ...
  }
  ```

- container

  ```scss
  @include container($bpMobile);
  ```

- column

  ```scss
  // column(size: int, numberOfColumns: int, breakpoint: int)
  @include column(1, $mobileTotalColumns, $bpMobile);
  ```

- custom-property

  ```scss
  // set margin to be equal to the total width of two columns
  @include custom-property(2, $mobileTotalColumns, margin-left);
  ```

- grid-container

  ```scss
  @include grid-container();
  ```

- nested-grid-container

  ```scss
  @include nested-grid-container();
  ```

# CSS grid

## Available classes
  - sufixes:
    - mobile
    - phablet
    - tablet
    - desktop
    - largeDesktop
    - xLargeDesktop

  - col-[column width]-[sufix]

### example:
```html
  <div class="container">
      <div class="grid">
        <div class="col-1-mobile col-3-desktop your-custom-class">sample</div>
        <div class="col-1-mobile col-3-desktop">sample 1</div>
        <div class="col-1-mobile col-3-desktop">sample 2</div>
        <div class="col-1-mobile col-3-desktop">sample 3</div>
      </div>
  </div>
```
