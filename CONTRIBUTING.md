# Contributing

Thanks for your interest in contributing.

## Development setup

1. Fork and clone the repository.
2. Open `chrome://extensions`.
3. Enable **Developer mode**.
4. Load this directory as an unpacked extension.

## Making changes

- Keep the extension CSS-only unless there is a clear need otherwise.
- Keep URL matches and selectors as narrow as possible.
- Avoid broad selectors that may hide unrelated content.

## Testing

- Test all currently supported URLs listed in `manifest.json`.
- Confirm SSN value is hidden.
- Confirm login content and flow are still usable.

## Pull requests

- Describe the reason for the change.
- Include affected URL patterns/selectors.
- Include manual verification notes.
