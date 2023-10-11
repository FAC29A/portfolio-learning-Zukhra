# Markup
This topic is focused on the fundamental building blocks of web pages—accessible, semantic HTML, and well-organised CSS.

## Git workflow

1. **Creating a New Repository:**
   - Setting up a new GitHub repository where your project code will be hosted.
     
2. **Clone this new repository using your terminal:**
   ```
   git clone 'PASTE THE URL OF YOUR REPOSITORY HERE'
   ```

2. **Issue Tracking:**
   - Using GitHub issues to track tasks and features to be implemented in the project.

3. **Branching:**
   - Creating separate branches for different features or tasks to ensure isolated development.
     ```
     git branch branch-name
     ```
   - Leave the main branch by switching to the new branch you have just created.
     ```
     git checkout branch-name
     ```
     Alternatively you can do this in a single step by using the -b flag to tell the git checkout command to create the new branch:
     ```
     git checkout -b branch-name
     ```   

4. **Committing Changes:**
   - Making changes to code files and committing them with descriptive commit messages.

5. **Pushing to Remote:**
   - Pushing your branch's changes to the remote GitHub repository.
     ```
     git push origin branch-name
     ```

6. **Pull Requests (PRs):**
   - Creating pull requests to propose changes to the **main** branch.
   - Reviewing PRs for code quality, correctness, and adherence to coding standards.

7. **Merging PRs:**
   - Merging approved pull requests into the main branch once they have been reviewed and approved.

8. **Handling Merge Conflicts:**
   - Resolving conflicts that occur when multiple branches modify the same code.

9. **Collaboration:**
   - Collaborating with team members by assigning tasks, reviewing code, and ensuring a smooth workflow.

11. **Best Practices:**
    - Following best practices for writing descriptive commit messages, linking commits to related issues, and maintaining a clean Git history.

Link to the work shop: https://learn.foundersandcoders.com/workshops/git-workflow/


## CSS layout

### Flow Layout

Flow layout is the default behavior of elements in CSS. It defines how block and inline elements are positioned within a document. Key points about flow layout:

- Block elements (e.g., div, header, p) take up the full width of the page.
- Inline elements (e.g., span, strong, a) occupy only as much horizontal space as needed.
- The viewport scrolls vertically when content overflows the screen.
- Content that is too wide for the viewport wraps elements onto the next line.

### Grid and Flexbox

CSS offers powerful layout tools in the form of grid and flexbox. These layouts provide greater control and flexibility in arranging elements. Key points:

- Grid layout allows you to create complex, grid-based designs.
- Flexbox is excellent for arranging elements in a single row or column.
- Both grid and flexbox layouts can adapt to different screen sizes.

### Centering Content

Centering content is a common layout task. You can achieve this using various techniques, such as:

- Setting `margin-left` and `margin-right` to `0` to constrain content width.
- Using `text-align: center` for centering inline elements.
- Applying flexbox or grid centering properties for more complex layouts.

### Using Variables and Root to Style CSS

CSS variables and the `:root` pseudo-class provide a convenient way to define and manage styles. Key points:

- Define CSS variables at the root level using `:root`.
- Access and utilize variables within your stylesheet to apply consistent styles.
- CSS variables make it easier to maintain and update styles.
```css
/* Define CSS variables at the :root level */
:root {
  --primary-color: #3498db;
  --font-family: 'Arial', sans-serif;
}

/* Utilize the defined variables in your stylesheet */
body {
  background-color: var(--primary-color);
  font-family: var(--font-family);
}
```

### Managing Spacing with a Parent Element (Stack)

One of the fundamental aspects of layout design is controlling the spacing between elements. To enhance reusability and maintain simplicity, it's often a good practice to avoid applying spacing rules directly to individual elements.

 A more flexible approach is to create a parent element that manages the spacing for its children. This common pattern is often referred to as a "stack." While various layout techniques (such as flexbox or grid) can be used to implement stacks, I'll illustrate a simple approach using margins.

```css
/* Apply a top margin of 1rem to all elements inside .stack */
.stack > * {
  margin-top: 1rem;
}

/* Special handling for the first child element inside .stack */
.stack > *:first-child {
  margin-top: 0; /* Remove the top margin to avoid extra spacing above the first element */
}
```

Link to the work shop: https://learn.foundersandcoders.com/workshops/css-layout/


## Semantic HTML

**Semantic HTML** is all about using the right HTML elements to convey the structure and meaning of your content, rather than just its appearance. It's essential for several reasons:

1. **Default Styles:** Browsers provide built-in styles for standard HTML elements. By using them, you save time and ensure your page still looks good even if your CSS fails.

2. **Complex Behavior:** Browsers handle intricate interactions like button clicks and keyboard actions. Relying on semantic elements saves you from reinventing the wheel.

3. **Machine-Readable:** Semantic HTML allows browsers and software to understand your content. It's critical for accessibility, ensuring that tools like screen readers can interpret your page correctly.

### Implementing Semantic HTML

To make your HTML more semantic:

- Use block elements like `<header>` and `<footer>` for meaningful page sections.
- Employ heading tags like `<h2>` and `<h3>` to structure your content.
- Utilize the `<a>` element for links to other pages.
- Choose `<button>` for elements triggering JavaScript behavior.
- Use `<form>` along with `<input>` and include `<label>` for user input forms.
- For layout or styling, you can use non-semantic elements like `<div>` and `<span`.

By following these guidelines, you create more accessible and meaningful web pages.

Link to the work shop: https://learn.foundersandcoders.com/workshops/semantic-html/

