# Astro Starter Kit: Minimal

```sh
npm create astro@latest -- --template minimal
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/minimal)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/minimal)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/minimal/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Notes to self

### Reason for using Videos vs GIF
A GIF recording of a mockup can come out to about 15-20mb for a 15 second clip related to a web application. On the other hand a properly encoded mp4 of it will only be 2mb. Due to bandwith limitations with netlify (100GB per month) it is much more reasonable to use these mp4s with proper coding.

I have found that using the built in screen record on mac to work fine for recording these. Using the application "handbrake" with preset H.264 MKV 2160p60 4k, format MP4, and Web Optimized, we can convert these to smaller mp4 files that also fix a looping bug found in web browsers. If the file does not shrink down to around 2mb, use vlc to convert mov file to mp4 first and then use preset on handbrake.


### Scripts being used
There is currently a script at the end of the case study layouts that fixes a bug between viewtransitions api and video loading. Basically the script just makes the video fully load after the view transitions is completed.

There are scripts being used for the home page  that seem to only work with view transitions enabled currently as well. This may break in the future, but hopefully not.


### Container Sizing
I recently shifted from 1fr 1.33fr to 1fr 1.5fr -- I should test this out and experiment if the sizing is too small for the left view. Currently it still doesn't feel like just a sidebar