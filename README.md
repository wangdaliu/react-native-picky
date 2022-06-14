# ⛏️ react-native-picky

An awesome native wheel picker component for react-native.

## Features

- Supports multiple columns ✅

- Supports looping ✅

- Native Android and iOS components for improved performance ✅

- Typescript ✅

## Preview

| Preview                       | iOS                                                      | Android                                                      |
| ----------------------------- | -------------------------------------------------------- | ------------------------------------------------------------ |
| Single Column                 | <img src="./docs/ios-single-column.gif" width="150">     | <img src="./docs/android-single-column.gif" width="150">     |
| Multiple Columns with looping | <img src="./docs/ios-multi-column-loop.gif" width="150"> | <img src="./docs/android-multi-column-loop.gif" width="150"> |

## Installation

```sh
yarn add react-native-picky
```

## Quick Start

```tsx
import { Picker, PickerGroup, PickerItem } from 'react-native-picky';

export const Demo = () => (
  <Picker>
    <PickerGroup>
      <PickerItem label="Monday" value="Monday" />
      <PickerItem label="Tuesday" value="Tuesday" />
      <PickerItem label="Wednesday" value="Wednesday" />
      <PickerItem label="Thursday" value="Thursday" />
      <PickerItem label="Friday" value="Friday" />
    </PickerGroup>
  </Picker>
);
```

## Props

### `<Picker />`

| Property       | Type     | Description                                               | Platform     | Default              |
| -------------- | -------- | --------------------------------------------------------- | ------------ | -------------------- |
| loop           | boolean  | Enable looping options                                    | iOS, Android | false                |
| style          | object   | View style prop                                           | iOS, Android |                      |
| onChange       | function | A callback function when a value is changed in any column | iOS, Android |                      |
| hasCurtain     | boolean  | Enable the curtain to highlight the selected value        | Android      | true                 |
| curtainColor   | string   | Color of the curtain                                      | Android      | hsla(0, 0%, 0%, 0.1) |
| hasIndicator   | boolean  | Enable the indicator to highlight the selected value      | Android      | true                 |
| indicatorColor | string   | Color of the indicator                                    | Android      | hsla(0, 0%, 0%, 0.1) |
| indicatorSize  | number   | The size of the indicator                                 | Android      | 1                    |
| itemSpace      | number   | The amount of space between items                         | Android      | 12                   |
| textColor      | string   | The color of the item text                                | Android      | #000000              |
| textSize       | number   | The size of the item text                                 | Android      | 20                   |

### `<PickerGroup />`

| Property      | Type             | Description                                               | Platform     | Default |
| ------------- | ---------------- | --------------------------------------------------------- | ------------ | ------- |
| selectedValue | string \| number | The selected value                                        | iOS, Android |         |
| onChange      | function         | A callback function if the value is changed in this group | iOS, Android |         |

### `<PickerItem />`

| Property | Type             | Description                | Platform     | Default |
| -------- | ---------------- | -------------------------- | ------------ | ------- |
| label    | string           | The label of the item      | iOS, Android |         |
| value    | string \| number | The value of the item      | iOS, Android |         |
| testID   | string           | The testID of the item     | iOS          |         |
| color    | string           | The color of the item text | iOS          |         |

## Contributing

See the [contributing guide](CONTRIBUTING.md) to learn how to contribute to the repository and the development workflow.

## License

MIT
