# GenericPopovers

**Reusable, themeable popover and alert views for UIKit**, built from one base class so every popover in an app shares the same header, card style, and close behaviour.

<p>
  <img alt="Swift" src="https://img.shields.io/badge/Swift-5.0-orange?style=flat-square">
  <img alt="UIKit" src="https://img.shields.io/badge/UIKit-popovers-blue?style=flat-square">
  <img alt="Built" src="https://img.shields.io/badge/Built-2018----2020-lightgrey?style=flat-square">
</p>

![Generic popovers demo](https://user-images.githubusercontent.com/23718584/48245298-37cbab80-e43e-11e8-9a71-5518b8ceec66.gif)

## What it demonstrates

- A `PopOverBaseViewController` with a reusable header template: card colour, title, and subtitle are configurable per popover
- Subclasses override stored properties (title, subtitle, content height) and add their own content view: image, table, or text input
- A `closePressedCallback` contract so every subclass dismisses consistently
- Keyboard-aware text input popovers that shift their content when needed
- Custom fonts and shared theming through a small `Utils` helper

## Project structure

```
PopOver/
├── PopoverBaseViewController.swift   Base class: header, card, close callback
├── PopOverSubClasses.swift           Image, table and input popovers
├── PopOverCallingClass.swift         Example of presenting each popover
└── Utils.swift                       Colours, fonts and helpers
```

## Running it

Open `GenericPopovers.xcodeproj` in Xcode and run on an iPhone simulator. The popovers were designed for portrait without Auto Layout, so keep size classes off in the subclasses' storyboards.

This project was later turned into a reusable framework: **[SwiftGenericAlertViewController](https://github.com/shruezee/SwiftGenericAlertViewController)**.

---

Built by **[Shruthi](https://github.com/shruezee)**, iOS developer in Sydney. See my latest apps: **[KindDose](https://github.com/shruezee/KindDose)** and **[MiniMingle Games](https://github.com/shruezee/MiniMingle-Games)**.
