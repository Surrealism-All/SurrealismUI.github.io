# Components(Wdigets)

- `SText` ：It is the simplest and most common component in SurrealismUI
- `SButton` ：`SButton` is a button component that you can freely perform regular attribute operations on
- `SIcon` ：this is a icon container , better than Image
- `SInput` ：This is a basic input box, often used in forms, divided into two types: text and password
- `SCard` ：A very simple universal card without any layout or restrictions ， you can add anything you want to the card
- `SStar` ： `SStar` is a scoring component
- `SSelect` ：`SSelect` is a selector that provides three types of optional input parameter values
- `STag` ：A small tag used to display data
- `SHeader` ：`SHeader` is a simple header component that is generated based on routing information
- `STable` ：In fact, it is just the header of the table and needs to be used together with `STableColumn` or `STableColumnFlex`

  - `STableColumn` ：It is table body , it covers the data of the table , It is easy for just show text in Table
  - `STableColumnFlex` ：It is also a kind of table body , but this component is more flexible , you can use with `STableColumnItem` together and define what will show in the table
  - `STableColumnItem` ：It is a component used to describe a cell in a table , It can help you define tables more easily.

- `SCollapse` ：`SCollapse` is a foldable panel. This is the outter of the Collapse, what really works is `SCollapseItem`. The outter only serves as a standard layout , this is a zero cost construction

  - `SCollapseItem` ：`SCollapseItem` is a component of `SCollapse`, without which `SCollapse` will not work , You can customize the components or use the default text display method in it

- `SResult` ：`SResult` helps you easily build a quick prompt , you can build it in popup window
- `SAvatar` ：`SAvatar` is a avatar component that defaults to Icons.Avatar when there are no images available
- `SLink` ：`SLink` is commonly used to represent text connections or sharing
- `SDivider` ：A divider groups sections of content to create visual rhythm and hierarchy. Use dividers along with spacing and headers to organize content in your layout.
- `SPopup` ：A masked pop-up layer appears in the current window . And users will not be able to use the pop-up layer to cover the components under it. Clicking on the pop-up layer again will close it
- `SCollection` ：`SCollection` is an expandable box that can be zoomed in or out by clicking (internal can also be used)
- `SRadio` ：`Radio `let people select a single item
- `SBadge` ：`SBadge` is a quick way to display user status or events
- `SPersona` ：This component is used to display simple user introduction information
- `SProgress` ：`SProgress` is commonly used to display download progress or event processing progress . And you can fully control it through the progress property
- `STip` ：A tip provides supplemental, contextual information elevated near its target component
- `SLoading` ： This is a loading component that you can embed anywhere you want to add a loading animation
- `SDialog` ：`SDialogs` are used to confirm messages or events and display text
- `SMenu` ：`SMenu` is a menu bar located on the left side that you can quickly generate through the menu-data property
- `SSwitch` ：`SSwitch` is a switch used for simple judgment scenarios
- `SDrawer` ：Sometimes, the Dialogue component does not meet our needs , such as your form being too long, or if you need to temporarily display some documents, please use the `SDrawer`
- `SAlert` ：`SAlert` is used to display important prompt information on the page
- `SSwitchGroup` ：`SSwitchGroup` switch group can contain more switch cases
- `STree` ：`STree` can be used to display directory structure, forming a parent-child relationship, and can be easily displayed
- `SFile` ：`SFile` can help users present file selectors GUI
- `STab` ：provide tab functionality, so that users can switch between different content sections
- `SCheckbox` ：`SCheckbox` let people select multi items
- `SPopover` ：A customizable popover component designed to display contextual information or interactive content, attached to an element and floating above the UI. It supports various positions and can be shown or hidden programmatically.
- `SStep` ：The Step component visualizes the progress of a sequence by breaking it down into individual steps. It allows for custom theming and supports indicating the current, completed, and pending steps through visual cues.
- `SKeyBoard` ：A customizable keyboard component for various input types including numbers, alphabets, and computer keyboard layouts.
- `SPagination` ：A component designed for navigating through pages, providing options for customization and various interactions.
- `SCarousel`：The Carousel component is designed to display a sequence of images (or slides) that users can navigate through. It provides a dynamic and visually engaging way to showcase multiple images without occupying too much space on the screen.
- `STimeLine`：The timeline component is mainly used to display the changes of data over time, and it is usually used in data visualization to visually represent time series data
- `SNumberInput`：A numeric input component that inherits from SCard, designed for inputting numerical values within a specified range. It allows adjustments through increment and decrement actions.
- `SCalendar`：A calendar component that inherits from SCard. It is designed to display a month view with the ability to navigate and select dates.