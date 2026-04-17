# Profile Card - Stage 1B

## Live Demo
https://hngi14-frontend-stage1b-profile-card.netlify.app/

## Features
- ✅ Semantic HTML5 (article, header, nav, section, figure)
- ✅ Full keyboard accessibility
- ✅ WCAG AA color contrast
- ✅ Responsive design (mobile → desktop)
- ✅ Live epoch timestamp (updates every 300ms for test accuracy)
- ✅ Social links open in new tabs with security attributes
- ✅ All required data-testid attributes

## Critical Fixes Applied
- Time updates every 300ms (not 1000ms) to pass test accuracy requirements
- Social links test ID on `<nav>` for robustness
- `aria-label` on name for screen readers
- Clean responsive behavior with proper flex breakpoints

## data-testid Reference
| Test ID | Element |
| test-profile-card | Card container |
| test-user-name | User name (with aria-label) |
| test-user-bio | Biography |
| test-user-time | Epoch milliseconds (updates every 300ms) |
| test-user-avatar | Avatar image |
| test-user-social-links | Social links nav container |
| test-user-social-twitter | Twitter link |
| test-user-social-github | GitHub link |
| test-user-social-linkedin | LinkedIn link |
| test-user-hobbies | Hobbies list |
| test-user-dislikes | Dislikes list |

## Accessibility
- Meaningful alt text on avatar
- `aria-live="polite"` for time updates
- Visible focus outlines
- Keyboard navigable
- `target="_blank"` + `rel="noopener noreferrer"`
- `aria-label` on name and social links

## Responsive Breakpoints
- Mobile: <640px (stacked, centered)
- Tablet: 641-768px (hybrid)
- Desktop: >768px (avatar left, content right)
