# Contributing

Thanks for taking an interest. Contributions are welcome: setting fixes, theme corrections and
guide improvements.

## What belongs here

- A wrong key or value in `settings.json`
- A config folder path that is wrong for a platform
- An extension id that is wrong or unpublished
- Improvements to the guides

## What does not belong here

- A setting or extension that only reflects one person's taste rather than something broadly
  useful, keep that in your own copy

## How to contribute

1. Fork the repository and create a branch named `fix/<short-description>` or
   `feat/<short-description>`.
2. Make your change and load it in a real Zed install to confirm it applies with no error. Zed
   accepts comments and trailing commas, so a strict JSON parser is not a valid check on its own.
3. Open a pull request with a clear title and a one-paragraph description of what changed and
   why. CI parses `settings.json` the way Zed does.

## Reporting bugs

Open an issue with your Zed version and platform, what you expected versus what happened.

More about me and my work: [isaacadjei.me](https://isaacadjei.me).
