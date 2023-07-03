```js
import { build } from "esbuild";
import { PostCssPlugin } from "@ikasoba000/esbuild-postcss-plugin";
import autoprefixer from "autoprefixer";

await build({
  entryPoints: ["src/index.css"],
  outdir: "./dist/",
  plugins: [
    PostCssPlugin({
      plugins: [autoprefixer()],
    }),
  ],
});
```
