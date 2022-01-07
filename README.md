# 0x0B. Implement a design with bootstrap

-   By Nicolas Philippot, UI/UX designer and Guillaume Salva, CTO at Holberton School

In this project, you will implement 3 web pages with Bootstrap. You will use all HTML/CSS/Accessibility/Responsive design/Bootstrap knowledges that you learned previously.

You won’t have a lot of instruction, you are free to implement it the way that you want - the objective is simple: Have fully functional web pages that look the same as the designer file.

Here the final result:

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/3c71cc99d2fc1c12a3d3.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=285bd9d1cfd9d0b15341c5d910eee857fb7c8e6f230d3bbc768e74cb8f1c6e14)

This webpage has been designed by Nicolas Philippot, UI/UX designer. You can find final screens  [here](https://intranet-projects-files.s3.amazonaws.com/holbertonschool-webstack/623/Archive.zip "here")

### Requirements

-   You have to use Bootstrap
-   Your  `styles.css`  must be as small as you can -  **you must use as much as you can Bootstrap classes**

### Imports

For this project, you will need: fonts from Google, JQuery, Bootstrap CSS/JS

```
<link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Coiny&display=swap" rel="stylesheet">

<script src="https://code.jquery.com/jquery-3.4.1.min.js" integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo=" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>

<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">

```

## Tasks

### 0. Read and be familiar with Figma

mandatory

Create an account in  [Figma](https://intranet.hbtn.io/rltoken/0OS4ME4Kjnw0I82IVkkoSw "Figma")  and open these files:

-   [Homepage](https://intranet.hbtn.io/rltoken/RLej4Ua6W3EmDh7UCwGTzQ "Homepage")  -  [fig file](https://intranet.hbtn.io/rltoken/1ZTxYF-usvxpIjj44YYcyw "fig file")
-   [Pricing](https://intranet.hbtn.io/rltoken/xQCL77_ePGWntUAe4T7ebQ "Pricing")  -  [fig file](https://intranet.hbtn.io/rltoken/AdJ6ZyZrG90gRNAI5bt_lA "fig file")
-   [Courses](https://intranet.hbtn.io/rltoken/__3w9ryapSUAwMaAYYS6ZA "Courses")  -  [fig file](https://intranet.hbtn.io/rltoken/1JL-gCkfJ5Hqb0Sf2lmymw "fig file")

And “Duplicate to your Drafts” to have access to all design details.

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/559ad8d43fb61e310e2b.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=bebad6f07c2cd2a05e430a862a6ae71126a498e924b591cee1e4d0b8ef39551d)

Important notes with Figma:

-   if your computer doesn’t have missing fonts, you can find them here:  [source-sans-pro](https://intranet.hbtn.io/rltoken/4uQkoVbAjr7lRVqSVCWBcw "source-sans-pro")  and  [Spin-Cycle-OT](https://intranet.hbtn.io/rltoken/5HnXzrMbtVKLCScrdy4CIg "Spin-Cycle-OT")
-   some values are in float - feel free to round them
-   “Be pixel perfect” - yes! but mainly make sure colors, size and position are correct.  #C271FF  is not  purple.

For this task, please write an amazing  `README.md`

**Interactions note:**

-   Web pages must switch to the tablet version when the screen width is 768px
-   Web pages must switch to the mobile version when the screen width is 576px
-   button hover/active:  `opacity: 0.9`

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `README.md`

Done?  Help

### 1. Header first

mandatory

Let’s start by the Homepage:  **create the header/hero piece**

Here an archive of all assets needed (for the entire project):

-   [images_images.zip](https://holbertonintranet.s3.amazonaws.com/uploads/misc/2020/3/e62e701b6ce0374555e9.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=345600&X-Amz-SignedHeaders=host&X-Amz-Signature=89f82e6b098c7601745cd64cb55e4786115f4d0c53ac257f29a9b61b1e030b51 "images_images.zip")
-   [holberton_school-icon.zip](https://holbertonintranet.s3.amazonaws.com/uploads/misc/2020/3/7159d988278de54d859d.zip?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=345600&X-Amz-SignedHeaders=host&X-Amz-Signature=b06d3f6230a0ed134b4e9dc34d081d0a2beaccf92cb6bafc7ab96d8a2a517257 "holberton_school-icon.zip")

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/4/13572c3773e26651761e8b4a74b3383300ed9563.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=88046ab956c695192c47bee6f826967b92331dea368dcc1fb0f4f9ea78ae9e4e)

**Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/8854d68a957ef7dc2315.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=614d3cda28aa8893943779657488190fe1a40212e55b9596f7ed729a4e8805e5)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `0-homepage.html, styles.css`

Done?  Help

### 2. Carousel of quotes

mandatory

**Create the section “Carousel of quotes”**

By using a Carousel component of Bootstrap, create this Carousel of quotes.

You can have for the moment one quote or twice the same for testing (like example below)

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/8455560f9ac188658195.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2f363e11183220528316c32127ce524871cc8e31bf32a2d7060b22946d844bc3)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `1-homepage.html, styles.css`

Done?  Help

### 3. Popular videos

mandatory

**Create the section “Most popular tutorials”**

By using a Carousel component of Bootstrap, create this Carousel of video cards.

**Reminder:**

-   Desktop: 4 cards
-   Tablet: 2 cards
-   Mobile: 1 card

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/4b610dc2d2cc17ceb2f7.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b1bb9aceba600571910011451b02511e6b99541f07cabe2c1b40e9dea968781b)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `2-homepage.html, styles.css`

Done?  Help

### 4. Row of smiles

mandatory

**Create the section “Free membership”**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/970efd54768b693bbfac.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2f8e32e509475d600f289199852e883fff98928426693b9f5d3fdd3f37b21a46)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `3-homepage.html, styles.css`

Done?  Help

### 5. Latest videos

mandatory

**Create the section “Latest videos”**

Copy the block “Most popular tutorials” to “Latest videos”

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `4-homepage.html, styles.css`

Done?  Help

### 6. ... and the footer!

mandatory

**Create the footer**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/739d7cc60098e7ff8f25.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=35073060df5bcfa36afd21772a2b02a07206ff2e66447bcf10f31047b5441f5a)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `homepage.html, styles.css`

Done?  Help

### 7. Pricing - header

mandatory

Now, let’s do the pricing page:  **create the header/hero piece**

The mobile version must be the same as the Homepage - it’s time to reuse code!

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/ccd30a4d80a990b96740.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=a109dfd4723e6fc8dd82492b2a4f7bb6fbef8be9ec79f215a59e259020b6e992)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `0-pricing.html, styles.css`

Done?  Help

### 8. Prices grid

mandatory

**Create the prices grid**

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/0ac3872946a0014e4f99.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=cd0705edaa8a1bf5ed4668703b3649e5535a3e0d6041e3701d3351ee35d3cbea)

**Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/edea8172b9cc0a867237.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=c06ffa4a2b10346f1c583227af65c13729e288d33520200db263acf3ee4351f7)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `1-pricing.html, styles.css`

Done?  Help

### 9. Quotes section

mandatory

Same as the Homepage,  **create the Carousel of quotes**

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `2-pricing.html, styles.css`

Done?  Help

### 10. FAQ

mandatory

**Create the FAQ grid**

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/db8f90e37593a29c1ab6.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d3c8b3ec1f25376d41ef83c8c58a800f49af038d5459c05eb504b47663a28044)

**Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/eaeb117d40690a451c7b.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=3fd8a4e194e2bc1fdf16b31c1e262e082eb60cb2e115ba0845979a3e8b5f3808)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `3-pricing.html, styles.css`

Done?  Help

### 11. Close the page with a footer

mandatory

Same as Homepage,  **create the footer**

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `pricing.html, styles.css`

Done?  Help

### 12. Courses - header

mandatory

Now, let’s do the courses page:  **create the header/hero piece**

The mobile version must be the same as the Homepage - it’s time to reuse code!

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/a5ba265af5dd643ad942.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6256f619a98ce264e10c84204ddf2af9b6a23ef93b37c279f2a7b9cfe6f65fa9)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `0-courses.html, styles.css`

Done?  Help

### 13. Search filters

mandatory

**Create the search filters section**

Dropdown is a nice way to create filters.

For the selected/placeholder value of both dropdown, no need to have dynamic value - static content is totally ok.

**Desktop:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/98c0564e59ec5620990e.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=98df49c4a0d2046c2dfd3c8dbed712eb344a1abf0c7662d0adac5be46a0cbc7d)

**Tablet/Mobile:**

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/3627550eccca7958d390.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=395117bb793f63676e818e6374f7047c17015fc603c003534f83fd0ab1c45b05)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `1-courses.html, styles.css`

Done?  Help

### 14. List of result

mandatory

**Create the result section of courses**

You can reuse the same cell for testing. Don’t forget to test with odd and even number of cells.

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/76b2074f3f6bbd25cdb9.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220107%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220107T195535Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8147e084884125c3b906a7d4692680f749d35a36beb6f20d91595465e250833d)

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `2-courses.html, styles.css`

Done?  Help

### 15. Close the page with a footer

mandatory

Same as Homepage and Pricing page,  **create the footer**

**Repo:**

-   GitHub repository:  `holberton-smiling-school`
-   File:  `courses.html, styles.css`