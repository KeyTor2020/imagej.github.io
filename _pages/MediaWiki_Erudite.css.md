/* Put the logo at the top of the page. */
#logo {
  position: absolute;
  top: 0;
  left: 0;
}

/* If screen is too narrow, make the logo more compact. */
@media screen and (max-width: 1056px) {
  #logo {
    width: 58px;
    top: -38px;
    left: 50px;
  }
}

/* Adjust the heading position. */
#top-wrap h1 {
  border: none;
  margin-left: 110px;
}

/* Hide the "From ImageJ" tagline */
#tagline {
  display: none;
}

/* Make the page manipulation links horizontal, and more compact. */
#nav-meta span {
  display: inline;
  padding-right: 1em;
}
#nav-meta {
  margin: 0;
}

/* Make the footer horizontal, and more compact. */
#footer {
  padding-right: 0;
}
#footer p {
  padding-right: 1em;
}
#footer li {
  display: inline;
  padding-right: 1em;
}

/* Move the search box to the top. */
li#search {
  font-size: 40.5px;
  position: absolute;
  right: 100px;
  top: -7px;
}
li#search h3 {
  display: none;
}

/* Hide the search box when the page is too narrow. */
@media screen and (max-width: 600px) {
  li#search {
    display: none;
  }
}

/* Box off the TOC like Vector does, to make it more consistent with other menu styling. */
.toc {
  background-color: #f9f9f9;
  border: 1px solid #a0a0a0;
  display: inline-block;
  padding: 0.5em 1em 0.5em 1em;
}

/* Make top-level headers small-caps, not all-caps. */
h1 {
  text-transform: none;
  font-variant: small-caps;
}

/* Underline the L1 and L2 headers, for readability. */
h1, h2 {
  border-bottom: 1px solid #a0a0a0;
  margin-bottom: 0.25em;
  overflow: hidden;
}

/* Do not underline the TOC heading, though. */
#toctitle h2 {
  border: none;
}

/* Make links brighter, and not underlined. */
a, a:visited {
  color: #26d;
  border: none;
}
/* Underline links during mouseover, though. */
a:hover {
  text-decoration: underline;
}

/* Fix padding of striped headers on front page. */
.header-stripe {
  padding-bottom: 0;
}

/* Make images + text middle aligned by default. See e.g. Introduction page. */
img {
  vertical-align: middle;
}

/* -- Template:Project styling -- */

/* Put the logo box on the top left of the page, below the main ImageJ logo. */
.project-info .project-logo {
  position: absolute;
  top: 178px;
  left: 35px;
  padding: 3px;
  border: 1px solid #ccc;
  background-color: white;
  border-radius: 1em;
  z-index: 100;
}
/* Make the logo image a nice size. */
.project-info .project-logo img {
  width: 48px;
  height: 48px;
  border: none;
  padding: 5px 5px 0 5px;
}

@media screen and (min-width: 1057px) {
  /* Use a nice drop shadow when page is wide enough. */
  .project-info .project-logo {
    -moz-border-radius: .75em;
    -webkit-border-radius: .75em;
    border-radius: .75em;
    -moz-box-shadow: 4px 4px 4px #ccc;
    -webkit-box-shadow: 4px 4px 4px #ccc;
    box-shadow: 4px 4px 4px #ccc;
  }
}
@media screen and (max-width: 1056px) {
  /* Put the logo box on the top of the page, next to the ImageJ title. */
  .project-info .project-logo {
    top: 4px;
    left: 220px;
  }
  /* Make the logo image a smaller size. */
  .project-info .project-logo img {
    width: 32px;
    height: 32px;
  }
}