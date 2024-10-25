# Learn Tailwind CSS - Scrimba
---

# **Tailwind CSS Documentation**

## **Background Classes & Shades**

In Tailwind CSS, the `bg-color-shade` class is used to set the background color of an element. For example, in the HTML code below, the `bg-gray-200` class provides a light gray background, while the `bg-white` class creates a white background. The `bg-blue-800` class is used to create a darker blue tone for the footer.

```html
<div class="bg-gray-200">Text1</div>
<div class="bg-white">Text2</div>
<div class="bg-blue-800">Text3</div>
```

## **Element Sizing & Tailwind's Numbering System**

In Tailwind CSS, `1 rem` represents `16 px`, which is the default font size. Therefore, using `1 rem` corresponds to a value of `4`. You can also use percentage values (like `1/2`, `3/1`, `2/5`) to size elements based on screen size. Additionally, you can assign "screen" or "full" as values for width or height.

```html
<div class="w-4">Text1</div>
<div class="h-2">Text2</div>
<div class="w-1/2">Text3</div>
<div class="w-screen">Text4</div>

```

## **Tailwind Padding & Margins**

To manage padding and margins, the format `m-number/p-number` is utilized. For example, the `ml-4` class adds a margin of 4 units to the left. You can also use the `x-y` format to create shorthand for the x-axis and y-axis.

```html
<div class="bg-blue-800 w-32 h-32 mb-4 pt-4 px-2">Lorem ipsum odor amet, consectetuer adipiscing elit.</div>
<div class="bg-blue-500 w-32 h-32 p-4">Lorem Ipsum</div>

```

## **Styling Text Part 1**

For text styling, you can set the font using `font-familyName`. Tailwind provides three main types of fonts: sans, serif, and mono. To apply the same font across all text elements, you can set it on the body tag.

For text size, the `text-size` class is used. Tailwind employs a special font sizing system. To align text, you can use the `text-alignment` class (left, right, center, justify). The `bg-color-shade` class can also be used to add a background color to text.

## **Styling Text Part 2**

To make text italic, the `italic` class can be used. For making a specific part of the text italic or not italic, you can use the `not-italic` or `italic` classes within a `span`.

The `font-weight` class allows you to set various weights (like thin, light, normal, or numerical values: 100, 200, 300, 400, etc.).

The `tracking-spacing` class is used for letter spacing, which is based on `em` units, not `rem`. The `em` unit is relative to the font size of the parent element, not the document.

The `leading` class is utilized for line spacing. Other text styling classes include `.underline`, `.no-underline`, `.line-through`, `.uppercase`, `.lowercase`, `.capitalize`, and `.normal-case`.

## **Borders**

To set border thickness, the `border-thickness` class is used (0, EMPTY, 1 (= px), 2, 3, 4, 5...).

The `border-side-thickness` class can be used to define the thickness for specific sides (left, right, top, bottom).

You can set border color with the `border-color-shade` class and border style with the `border-style` class (solid, dashed, dotted, double, none).

For rounded borders, the `rounded-radius` class can be applied, allowing you to set custom rounding. For instance, `round-2xl` means two times the standard rounding.

## **Display Modes**

Tailwind provides several classes to control the display properties of elements, making it easy to control visibility and layout types.

•	block: Sets an element to display as a block, taking up the full width of its parent container.

•	inline-block: Displays an element as an inline-level block container. It allows elements to sit next to each other on the same line while still respecting width and height properties.

•	inline: Sets an element to display inline, meaning it won’t start a new line and takes up only as much width as its content.

•	flex: Activates Flexbox layout, allowing flexible alignment, distribution, and ordering of items within the container.

•	inline-flex: Displays an element as an inline-level flex container, allowing it to align with other inline elements.

•	grid: Enables CSS Grid layout, which allows for a two-dimensional layout of items with rows and columns.

•	inline-grid: Applies a grid layout on an inline element, useful for aligning grid containers with inline elements.

•	hidden: Completely hides the element, removing it from the visual flow of the page.

•	table: Displays an element as a table, similar to the default styling of an HTML <table> element.

•	table-row and table-cell: Used for building table structures in CSS, allowing flexibility in layouts that resemble traditional tables.

These display classes enable quick adjustments to how elements are positioned and visualized within your layout, making Tailwind CSS an efficient choice for responsive and flexible design.

## **Flexbox**

The `flex` class is used to activate the Flexbox layout for elements in Tailwind.

### **Justify Alignment**

Use `justify-alignment` to align elements horizontally within the flex container. Options include `justify-start`, `justify-center`, `justify-end`, `justify-between`, and `justify-around`.

### **Item Alignment**

The `item-alignment` property aligns items vertically within the flex container. Options include `items-stretch`, `items-start`, `items-center`, `items-end`, and `items-baseline`. Note that using `items-stretch` (the default setting) makes each item take up the full height of the container, whereas `items-start` makes items only take up the space required by their content.

### **Flex Direction**

The `flex-direction` class defines the direction of elements in the flex container: `flex-row` (default), `flex-row-reverse`, `flex-col`, and `flex-col-reverse`.

### **Flex Wrap**

The `flex-wrap` property controls wrapping behavior. Options include `flex-no-wrap` (default), `flex-wrap`, and `flex-wrap-reverse`.

## **Responsive Design**

Tailwind allows for responsive design using breakpoint-specific classes. Breakpoints include:

- `sm` (640px)
- `md` (768px)
- `lg` (1024px)
- `xl` (1280px)

You can apply responsive versions of classes like `bg`, `w`, `h`, `m`, `p`, `font`, `border`, `display`, and `flex`.

## **Hover Effects**

To add hover effects, use the `hover:` prefix with any class, such as `hover:bg-blue-500`.

## **Focus Effects**

To style elements on focus, use the `focus:` prefix, such as `focus:border-blue-500`.

## **Combination Modifier**

Classes can be combined with modifiers, such as `md:hover:bg-red-500`, to apply styles when the screen is medium-sized and the element is hovered.

## **Other Utilities**

- **Shadow Size**: Use `shadow-md`, `shadow-lg`, `shadow-xl`, and `shadow-2xl` for various shadow effects.
- **Opacity**: Set element opacity with percentage values like `opacity-50`.
- **Cursor**: Control the cursor style (refer to Photo 0.8 for details).
- **Selection**: Control text selection behavior using classes like `select-none`, `select-text`, `select-all`, and `select-auto`.
- **Screen Reader Only**: Use `sr-only` for accessible text that only screen readers detect, and `not-sr-only` to reveal it.

## **Gradients**

Creating a gradient in Tailwind requires three classes:

- **`bg-gradient-{position}`**: Defines the position of the gradient (refer to Photo 0.9 for visual reference).
- **`from-{color}`**: Specifies the starting color of the gradient.
- **`to-{color}`**: Specifies the ending color of the gradient.

## **Fill**

The `fill-{color}` class is used to apply color to SVG elements, filling them with the specified color.

## **Marker**

The `marker:text-{color}` class is used to set the color of list markers, such as bullets or numbers, within lists.

## **Grid**

To create grid layouts, use the following classes:

- **`grid`**: Initializes the grid layout.
- **`grid-rows-{number}`**: Defines the number of rows in the grid.
- **`grid-cols-{number}`**: Defines the number of columns in the grid.
- **`gap-{number}`**: Sets the spacing between grid items.
- **`grid-span-{number}`**: Determines how many rows or columns an element should span within the grid.

## **Background Images in TailwindCSS**

Tailwind allows you to use images as background with these classes:

- **`bg-{file}`**: Sets the background image.
- **`md:bg-{file}`**: Sets the background image on medium screens and up.
- **`bg-no-repeat`**: Prevents the background image from repeating.
- **`bg-left-bottom`**: Positions the background image to the left bottom of the container.
- **`bg-fixed`**: Fixes the background image in place, making it stay relative to the viewport instead of scrolling with the page.

## **Transformations**

Transformation classes allow for modifications like scaling, rotating, and translating elements:

- **`scale-{number}`**: Scales the element by the specified factor.
- **`scale-x/y-{number}`**: Scales the element along the X or Y axis.
- **`rotate-{number}`**: Rotates the element by a specific degree.
- **`translate-x/y-{number}`**: Moves the element along the X or Y axis by the specified amount.

## **Transitions**

Tailwind’s transition classes enable smooth effects when elements change states:

- **`transition-{property}`**: Specifies which properties should transition (e.g., `all`, `none`, `color`, `opacity`, `scale`).
- **`duration-{number}`**: Sets the duration of the transition in milliseconds.
- **`delay-{number}`**: Adds a delay before the transition starts.

## **Arbitrary Values**

The `class-[property]` syntax in Tailwind allows you to set custom values for properties, offering flexibility for unique styling needs.

```html
<div class="w-[25px]">Text1</div>
<div class="h-[3rem]">Text2</div>
<div class="bg-[#ffffff]">Text3</div>

```
