# dropdown-calendar-shadcn-fix
A fix for Shadcn calendar component when used with dropdown for easy navigation. 
The default shadcn calendar component uses React-Day-Picker library but when we use it with the prop, `captionLayout="dropdown-button"` / `captionLayout="dropdown"`, we get a broken UI.

### Note
The [code](https://github.com/tathagat-m/dropdown-calendar-shadcn-fix/blob/main/dropdownCalendar.jsx) in this repository is not intended to be a direct replacement for the Shadcn "calendar" component, as doing so would alter the behavior of the range mode and could result in a broken UI. Instead, I recommend creating a separate component named "dropdownCalendar" and using the provided code for that component. This new component can be used wherever a single date selection is needed with a dropdown for Month and Year. For scenarios where a date range is required or a dropdown is unnecessary, the original "calendar" component from Shadcn should still be used.

***The idea and inspiration for this repo comes from [WebDevEducation](https://www.youtube.com/@WebDevEducation), particularly from this [video](https://www.youtube.com/watch?v=cY5RMVj2GtU).***

# Integration

## Prerequisites
- You should have a working project with Shadcn configured.
- You should have already installed Shadcn [Calendar](https://ui.shadcn.com/docs/components/calendar) & Shadcn [Select](https://ui.shadcn.com/docs/components/select).
- If you haven't completed these steps, please set them up before proceeding.

## Steps
- By default, Shadcn installs the components into the `src/components/ui` directory. Navigate to this folder, or to the location where you have configured Shadcn to install components.
- Create a new file named `dropdownCalendar.tsx` or `dropdownCalendar.jsx`, depending on whether you use TypeScript in your project.
- Copy the code from this [file](https://github.com/tathagat-m/dropdown-calendar-shadcn-fix/blob/main/dropdownCalendar.jsx) into the newly created file.
- Done! You can now import `DropDownCalendar` instead of `Calendar` wherever you need dropdowns for Month and Year.
- You can still import and use `Calendar` in places where dropdowns are not needed. This will also not break your existing `Calendar` implementations.



**If you find this repository helpful, please give it a ⭐️! Your support is greatly appreciated and helps others discover this project.**
