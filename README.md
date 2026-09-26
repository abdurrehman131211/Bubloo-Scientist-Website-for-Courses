# Bubloo Scientist Academy — AI That Actually Works

Static course website for Bubloo Scientist Academy.

## Registration
The public website has **no form configuration UI** and does not allow visitors to change the registration destination. The registration form is fixed in `app.js`:

```js
const REGISTRATION_FORM_URL='https://forms.gle/tFkcedja3DEHco8T6';
```

Learners can fill the embedded Google Form or open it in a new tab. Responses are handled by Google Forms and can be reviewed in the organizer's Google Sheets response destination.

## Deploy
Upload the `bubloo-course-site` folder to any static hosting provider such as Vercel, Netlify, GitHub Pages, or Cloudflare Pages.

## Included
- Responsive Bubloo Scientist Academy landing page
- 7-lesson interactive course viewer
- Practical exercises and quizzes
- Local lesson completion state
- Registration section with fixed Google Form
- Course workbook and audio scripts
- Quiz bank and instructor guide
