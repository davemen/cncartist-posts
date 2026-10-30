# cncArtist posts

Post processors for [cncArtist](https://cncartist.app), one file per machine.

A post decides how cncArtist writes G-code for your controller: units, comments, tool changes, spindle and the start and end of the file. Every post here is a plain JSON file ending in `.cncpost`.

## Use a post

1. Download the `.cncpost` file for your machine from [posts/](posts/).
2. In cncArtist, open the job's **Post** menu and choose **Import a post (.pp or .cncpost)…**.
3. Check the sample output in the editor, then save.

The post menu already includes every post in this repository; download from here only if you want a newer version.

## Add or fix a post

1. In cncArtist, choose **Copy and edit…** on the closest post, change it, and cut a test piece in air first.
2. Choose **Share as a file…** to save it as a `.cncpost`.
3. Open a pull request that adds it to `posts/`, with:
   - the machine and controller (and its firmware version),
   - what you cut with it,
   - a short G-code file it wrote that ran well.

Not sure how? Use **Request a post…** in the app, or email support@cncartist.app with your machine, controller and a G-code file that already runs on it.

## Safety

Run every new post in air, with the spindle off and the bit well above the work, before you cut. A post that is wrong can drive the bit into the table or clamps. Posts are shared as-is, without warranty.

## Licence

The posts are released under CC0 1.0: use them for anything.
