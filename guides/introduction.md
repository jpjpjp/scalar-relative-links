# Relative Links in Scalar Docs

This page explores how, or if, relative links work in a scalar doc.

## Links to images

### Relative links

Classic relative links, which help make the project portable, for example it will run locally with `scalar project preview` and when publishing to scalar hosting, don't seem to work, at least the way I'm using them.

Below is a link to an image in a sister directory using the classic markdown relative link syntax, ie `![Copy Data](../images/CopyCategoriesAndTags.jpg)`

![Copy Data](../images/CopyCategoriesAndTags.jpg)

And here is a link to the same image using HTML, ie:
```html
<scalar-image
  src="../images/CopyCategoriesAndTags.jpg"
  alt="Copy Data">
</scalar-image>
```
<scalar-image
  src="../images/CopyCategoriesAndTags.jpg"
  alt="Copy Categories and Tags">
</scalar-image>

### Absolute links

Absolute links do seem to work, but the tightly couple the project to a particular URL

```md
![Copy Data](https://raw.githubusercontent.com/jpjpjp/lm-v2-dev-portal-poc/refs/heads/main/images/CopyCategoriesAndTags.jpg)
```
![Copy Data](https://raw.githubusercontent.com/jpjpjp/lm-v2-dev-portal-poc/refs/heads/main/images/CopyCategoriesAndTags.jpg)

And here is a link to the same image using HTML, ie:
```html
<scalar-image
  src="https://raw.githubusercontent.com/jpjpjp/lm-v2-dev-portal-poc/refs/heads/main/images/CopyCategoriesAndTags.jpg"
  alt="Copy Categories and Tags">
</scalar-image>
```
<scalar-image
  src="https://raw.githubusercontent.com/jpjpjp/lm-v2-dev-portal-poc/refs/heads/main/images/CopyCategoriesAndTags.jpg"
  alt="Copy Categories and Tags">
</scalar-image>

## Links to other pages

### Relative links

Below is a link to a document in the same directory using the classic markdown relative link syntax, ie `[Another page](./other-page.md)`

Clicking on [this relative link to another page](./other-page.md) seems to load the current main page again.


### Absolute links

TBD 

## Questions

Does scalar support a relative link syntax?