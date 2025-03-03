## API Report File for "@fluentui/react-timepicker-compat"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import type { ComboboxProps } from '@fluentui/react-combobox';
import type { ComboboxSlots } from '@fluentui/react-combobox';
import type { ComboboxState } from '@fluentui/react-combobox';
import type { ComponentProps } from '@fluentui/react-utilities';
import type { ForwardRefComponent } from '@fluentui/react-utilities';
import * as React_2 from 'react';
import type { SelectionEvents } from '@fluentui/react-combobox';
import type { SlotClassNames } from '@fluentui/react-utilities';

// @public
export function formatDateToTimeString(date: Date, { hourCycle, showSeconds }?: TimeFormatOptions): string;

// @public
export const TimePicker: ForwardRefComponent<TimePickerProps>;

// @public (undocumented)
export const timePickerClassNames: SlotClassNames<TimePickerSlots>;

// @public
export type TimePickerErrorType = 'invalid-input' | 'out-of-bounds' | 'required-input';

// @public
export type TimePickerProps = Omit<ComponentProps<Partial<ComboboxSlots>, 'input'>, 'children' | 'size'> & Pick<ComboboxProps, 'appearance' | 'defaultOpen' | 'defaultValue' | 'inlinePopup' | 'onOpenChange' | 'open' | 'placeholder' | 'positioning' | 'size' | 'value' | 'mountNode' | 'freeform'> & TimeFormatOptions & {
    startHour?: Hour;
    endHour?: Hour;
    increment?: number;
    dateAnchor?: Date;
    selectedTime?: Date | null;
    defaultSelectedTime?: Date;
    onTimeChange?: (event: TimeSelectionEvents, data: TimeSelectionData) => void;
    formatDateToTimeString?: (date: Date) => string;
    parseTimeStringToDate?: (time: string | undefined) => TimeStringValidationResult;
};

// @public (undocumented)
export type TimePickerSlots = Omit<ComboboxSlots, 'clearIcon'>;

// @public
export type TimePickerState = ComboboxState & Required<Pick<TimePickerProps, 'freeform' | 'parseTimeStringToDate'>> & {
    submittedText: string | undefined;
};

// @public (undocumented)
export type TimeSelectionData = {
    selectedTime: Date | null;
    selectedTimeText: string | undefined;
    errorType: TimePickerErrorType | undefined;
};

// @public (undocumented)
export type TimeSelectionEvents = SelectionEvents | React_2.FocusEvent<HTMLElement>;

// @public
export const useTimePicker_unstable: (props: TimePickerProps, ref: React_2.Ref<HTMLInputElement>) => TimePickerState;

// @public
export const useTimePickerStyles_unstable: (state: TimePickerState) => TimePickerState;

// (No @packageDocumentation comment for this package)

```
