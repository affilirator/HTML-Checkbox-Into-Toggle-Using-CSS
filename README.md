# HTML-Checkbox-Into-Toggle-Using-CSS

## HTML Structure

- We use a `<label>` element to wrap the checkbox and the custom toggle.
- Inside the label, we have an `<input type="checkbox">` which is the actual form control.
- We add a `<span class="slider">` which will be styled to create the visual toggle.

## CSS Styling

1. `.toggle-switch`: This class styles the container for our toggle switch.
2. `input`: We hide the actual checkbox input by setting its opacity to 0 and dimensions to 0.
3. `.slider`: This creates the background of our toggle switch.
4. `.slider:before`: This creates the circular knob that moves when the toggle is switched.
5. `input:checked + .slider`: This selector applies styles when the checkbox is checked, changing the background color.
6. `input:checked + .slider:before`: This moves the knob to the right when the checkbox is checked.

## Accessibility

- By using a proper `<label>` element, we ensure that clicking on the toggle will change the state of the checkbox, making it accessible.
- The `:focus` pseudo-class adds a subtle box-shadow when the toggle is focused, providing a visual cue for keyboard navigation.

## Usage

To use this toggle in your project:

1. Copy the HTML for the toggle switch:

```html
<label class="toggle-switch">
  <input type="checkbox" />
  <span class="slider"></span>
</label>
```

2. Include the CSS in your stylesheet or within a `<style>` tag in your HTML document.
3. You can customize the colors, sizes, and transition speed by modifying the CSS variables.

This implementation creates a visually appealing toggle switch that users can interact with just like a regular checkbox. The underlying checkbox maintains its functionality, so it will work with forms and JavaScript as expected.
