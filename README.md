a very clumsy python API to create posts on bluesky (literally my first python project, and the posting logic is from bsky example tutorial)

publicly available here: 

`GET https://bluesky.stormycat.xyz/im_alive` => to check if it's alive

`POST https://bluesky.stormycat.xyz/create` => to create a post on BlueSky

Content-Type: 'application/json'

JSON body params: 
```
"pds_url": defaults to "https://bsky.social",
"handle": Your BlueSky handle,
"password": Your BlueSky password,
"text": the content of the post,
"image": URL for images in the post,
"alt_text": ALT text of the post,
"lang": Language of the post,
"reply_to": URL of a BlueSky post to reply to
"embed_url": URL of a website to be displayed as a website card on the post,
"embed_ref": I don't remember
```

The script for the posts comes from : https://atproto.com/blog/create-post
More information on everything there