Nivedha — Personal Portfolio Website

A single-page personal portfolio website built with pure HTML, CSS, and vanilla JavaScript. Designed with a dark luxury aesthetic, smooth scroll animations, and a fully responsive layout — no frameworks, no build tools, no dependencies.



Live Demo

> Open `nivedha-portfolio.html` directly in any modern browser — no server required.

---

Features

- **Fixed navigation** with active section highlighting on scroll and a mobile hamburger menu
- **Hero section** with animated scroll indicator, CSS grid texture background, and glowing orb effect
- **About section** with a pure CSS avatar placeholder and decorative offset border accent
- **Skills section** with sticky sidebar, pill-style skill tags, and animated proficiency bars
- **Projects section** with hover-lift cards, unique gradient thumbnails, and staggered fade-in animation
- **Contact section** styled as a macOS Mail-style inbox compose window with a title bar, tabs, meta rows, formatting toolbar, and send button
- **Scroll-triggered fade-up animations** using IntersectionObserver — plays once per element
- **Fully responsive** across desktop, tablet, and mobile with no external CSS framework

Tech Stack

| Technology |       | Purpose |
| HTML5              | Page structure and semantic markup |
| CSS3               | Styling, layout, animations, responsive design |
| Vanilla JavaScript | Scroll animations, mobile menu, form handling, nav highlighting |
| Google Fonts       | Cormorant Garamond (serif) + DM Sans (sans-serif) |
| Inline SVG         | Social icons (GitHub, LinkedIn, X, Instagram) |

Project Structure

nivedha-portfolio.html     ← entire project in one file
README.md


Since this is a single-file project, all HTML, CSS, and JavaScript are contained within `nivedha-portfolio.html`. No external stylesheets or script files are used.
Sections

| Section |      | Description |
| Hero           | Name, tagline, CTA buttons, animated scroll line |
| About          | Bio, CSS avatar, quick stats (projects, years, technologies) |
| Skills         | Core languages, frameworks, tools, proficiency bars |
| Projects       | 4 featured project cards with tags, description, and links |
| Contact        | Inbox-style compose UI with send functionality |
| Footer         | Logo, copyright, social media links |

 Projects Showcased

### ChatFlow — Real-Time Messenger
Multi-room chat application built with Java and WebSockets. Features user authentication and MySQL-backed chat history with a JavaFX desktop UI.
`Java` `Socket.IO` `MySQL`

### ZenScreen — Digital Wellbeing App
Glassmorphism-styled wellness app with SVG ring charts, Pomodoro timer, mood tracker, and a 7-day detox challenge.
`HTML` `CSS` `JavaScript`

### ShopEase — E-commerce UI
Responsive e-commerce front-end with product grid, filtering, cart sidebar, and mobile-friendly checkout flow.
`HTML` `Bootstrap` `CSS`

### StudentTrack — Grade Manager
Desktop application for managing student records and grades with MySQL backend and report generation.
`Java` `MySQL` `JavaFX`


## Skills Highlighted

**Core Languages** — HTML5, CSS3, JavaScript, Java

**Frameworks & Libraries** — React (Learning), Bootstrap, Tailwind CSS

**Tools & Workflow** — Git & GitHub, Figma, VS Code, MySQL


## Key Implementation Details

### CSS Custom Properties
All colors, fonts, spacing, and transitions are defined as CSS variables in `:root`, making the entire theme editable from a single block.

### Scroll Animations
Uses the native `IntersectionObserver` API to trigger fade-up animations when elements enter the viewport. Each element animates only once. Project cards use staggered `transition-delay` values to cascade in sequence.

### Responsive Layout
Built with CSS Grid (`grid-template-columns`) and Flexbox throughout. Two-column layouts collapse to single-column at 860px. Navigation switches from a link list to a hamburger menu at 640px. Typography uses `clamp()` for fluid scaling between breakpoints.

### Inbox Contact UI
The contact form is styled to resemble a macOS Mail compose window — complete with traffic-light window controls (red, amber, green dots), tab bar, structured meta rows (To, From, Name, Subject), a rich-text-style toolbar, and an animated send button with an embedded SVG icon.

### No Build Step Required
The entire project is one `.html` file. Open it in a browser and it works. Google Fonts is the only external resource (loaded via CDN link tag).



## How to Use

**1. Clone or download**
```bash
git clone https://github.com/yourusername/nivedha-portfolio.git
```

**2. Open in browser**
```bash
open nivedha-portfolio.html
# or just double-click the file
```

**3. Customize**

| What to change |     | Where to find it |

| Name and tagline     | `#hero` section in HTML |
| Bio text             | `#about` section in HTML |
| Accent color         | `--accent` in `:root` CSS variables |
| Skills list          | `#skills` section — add or remove `.skill-tag` elements |
| Projects             | `#projects` section — duplicate or edit `.project-card` blocks |
| Contact email        | `#contact` section — update the `.contact-item` and `inbox-meta-row` |
| Social links         | `<footer>` — replace `href="#"` with your actual profile URLs |

---

## Browser Support

| Browser|       | Support |

| Chrome 88+     |  Full |
| Firefox 78+    | Full |
| Safari 14+     |  Full |
| Edge 88+      |Full |

> `backdrop-filter` (frosted glass nav) is not supported in Firefox by default but degrades gracefully — the nav simply shows a solid dark background instead.


## Performance Notes

- Zero JavaScript dependencies — no jQuery, no libraries
- No CSS framework — no unused utility classes
- Fonts loaded from Google CDN with `display=swap` fallback behavior
- `IntersectionObserver` is used instead of scroll event listeners for animation triggering, which is significantly more performant
- All icons are inline SVG — no icon font or image HTTP requests


## Customization Tips

**To add a real profile photo:**
Replace the `.avatar-placeholder` div in the About section with:
```html
<img src="your-photo.jpg" alt="Nivedha" style="width:100%; height:100%; object-fit:cover;"/>
```

**To wire up the contact form:**
Replace the `handleSubmit()` function with a fetch call to a form backend like Formspree, EmailJS, or your own API endpoint.

**To change the color theme:**
Edit just these two variables in `:root`:
```css
--accent:  #c8a97e;   /* currently warm gold  — try #7eb8c8 for cool blue */
--accent2: #8fb8a0;   /* currently muted sage — try #b87eb8 for soft purple */
```

## Author

**Nivedha**
B.Tech — Computer Science | Tamil Nadu, India
Open to internships and freelance opportunities.

-  nivedha@example.com
-  [LinkedIn](#)
-  [GitHub](#)

## License

This project is open source and available under the [MIT License](LICENSE)

*Built with HTML, CSS & JavaScript — no frameworks, just fundamentals.*
