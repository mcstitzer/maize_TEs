# maize_TEs
TE annotations for multiple maize genomes

see [mcstitzer.github.io/maize_TEs](http://mcstitzer.github.io/maize_TEs) for a description of these files.

Remember to put new images in `/static/images` so that they get compiled with hugo

Having issues with css - fixed by changing 

`      <link href="/dist/css/app.e08a958ae3e530145318b6373195c765.css" rel="stylesheet">`
to
`      <link href="/maize_TEs/dist/css/app.e08a958ae3e530145318b6373195c765.css" rel="stylesheet">`

(```/maize_TEs/``` added to start ) on two lines (or one?) in `public/index.html` after hugo makes it by running `./publish_changes.sh` here.

To get the image at the top to run, have to manually change the url from:
`/maize_TEs/images/darkcorn.jpg`
to:
`https://github.com/mcstitzer/maize_TEs/blob/gh-pages/images/darkcorn.jpg`
