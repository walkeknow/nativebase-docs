---
id: switch
title: Switch
---

The `Switch` component is an alternative to the Checkbox component. You can switch between enabled or disabled states.

## Implements

- [`Switch`](https://reactnative.dev/docs/switch) from [`React Native`](https://reactnative.dev)

## Examples

### Basic

```SnackPlayer name=Switch%20Example
import React from 'react';
import { Switch, NativeBaseProvider, Center } from 'native-base';

function SwitchComponent () {
  return (
    <Switch />
  );
}

// Example template which wraps component with NativeBaseProvider
export default function () {
  return (
    <NativeBaseProvider>
      <Center flex={1}>
        <SwitchComponent />
      </Center>
    </NativeBaseProvider>
  );
}
```

### Sizes

```SnackPlayer name=Switch%20Sizes
import React from 'react';
import { Stack, Switch, NativeBaseProvider, Center } from 'native-base';

function SwitchComponent () {
  return (
    <Stack space={4}>
      <Switch size="sm" />
      <Switch size="md" />
      <Switch size="lg" />
    </Stack>
  );
}

// Example template which wraps component with NativeBaseProvider
export default function () {
  return (
    <NativeBaseProvider>
      <Center flex={1}>
        <SwitchComponent />
      </Center>
    </NativeBaseProvider>
  );
}
```

### Background

```SnackPlayer name=Switch%20Background
import React from 'react';
import { Stack,Switch, NativeBaseProvider, Center } from 'native-base';

function SwitchComponent () {
  return (
    <Stack space={4}>
      <Switch />
      <Switch offTrackColor="lightBlue.400" onTrackColor="emerald.400" />
      <Switch offThumbColor="lightBlue.400" onThumbColor="emerald.400" />
    </Stack>
  );
}

// Example template which wraps component with NativeBaseProvider
export default function () {
  return (
    <NativeBaseProvider>
      <Center flex={1}>
        <SwitchComponent />
      </Center>
    </NativeBaseProvider>
  );
}
```

## Props

| Name               | Type             | Description                                                                                          | Default |
| ------------------ | ---------------- | ---------------------------------------------------------------------------------------------------- | ------- |
| name               | string           | The input name of the Switch when used in a form.                                                    | -       |
| size               | `lg`, `md`, `sm` | The size (width and height) of the switch.                                                           | `md`    |
| isChecked          | boolean          | If true, set the Switch to the checked state.                                                        | -       |
| defaultIsChecked   | boolean          | If true, the checkbox will be initially checked.                                                     | -       |
| isDisabled         | boolean          | If true, set the disabled to the invalid state.                                                      | -       |
| isInvalid          | boolean          | If true, set the switch to the invalid state.                                                        | -       |
| onTrackColor       | string           | The track color of the Switch when on.                                                               | -       |
| offTrackColor      | string           | The track color of the Switch when off.                                                              | -       |
| onThumbColor       | string           | The thumb color of the Switch when on.                                                               | -       |
| offThumbColor      | string           | The thumb color of the Switch when off.                                                              | -       |
| onToggle           | function         | Function called when the state of the Switch changes.                                                | -       |
| accessibilityLabel | string           | [`Accessibilty label`](https://reactnative.dev/docs/accessibility#accessibilitylabel) for component. | -       |
| accessibilityHint  | string           | [`Accessibilty hint`](https://reactnative.dev/docs/accessibility#accessibilityhint) for component    |         |
