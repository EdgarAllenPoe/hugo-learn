+++
date = "2016-05-27T22:42:55-04:00"
draft = "false" 
title = "Understanding the use of archtype"

+++

By default when you execute the command `hugo new post/newpost.md` a file will be created in `content/post` directory with the following content:

```
+++
date = "2016-05-27T22:42:55-04:00"
draft = true
title = "newposte"

+++
```

But if you create a file named `post.md` in the archtype directory with the the following content:

```
+++
author = "authorsname"
co-author = "coauthorname"

+++
```

Then when you execute `hugo new post/nextpost.md`, becuase this file is created in the `post` sub-directory and because there is a post.md file in the `archtype` directory, the contents of the `nextpost.md` will be:

```
+++
date = "2016-05-27T22:42:55-04:00"
draft = true
title = "nextpost"
author = "authorsname"
co-author = "coauthorname"
+++
```


