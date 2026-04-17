# Advanced Todo Card - Stage 1A

## Live Demo
https://hngi14-frontend-stage1a-todo-card.netlify.app/

## Features
- ✅ Semantic HTML5 (article, form, label, select, time)
- ✅ Full keyboard accessibility
- ✅ WCAG AA color contrast
- ✅ Responsive design (mobile → desktop)
- ✅ Edit mode with save/cancel functionality
- ✅ Status transitions (Pending → In Progress → Done)
- ✅ Priority visual indicators (Low/Medium/High with colored dot + left border)
- ✅ Expand/collapse for long descriptions
- ✅ Overdue indicator with red accent
- ✅ Dynamic time remaining (updates every 30 seconds)
- ✅ Checkbox ↔ Status control synchronization
- ✅ All required data-testid attributes

## Critical Fixes Applied
- Time remaining stops updating when status becomes "Done" (shows "Completed")
- Cancel button restores previous values (backup system implemented)
- Edit mode returns focus to Edit button when closed
- Expand/collapse defaults to collapsed if description exceeds 100 characters
- Overdue indicator shows clear text (e.g., "⚠️ Overdue by 2 hours")
- Priority indicator uses both colored dot + left border accent
- In Progress state has distinct blue gradient visual style

## data-testid Reference

### Stage 0 Test IDs (Preserved)
| Test ID | Element |
|---------|---------|
| `test-todo-card` | Card container |
| `test-todo-title` | Task title |
| `test-todo-description` | Task description |
| `test-todo-priority` | Priority badge |
| `test-todo-due-date` | Due date |
| `test-todo-time-remaining` | Time remaining |
| `test-todo-status` | Status badge |
| `test-todo-complete-toggle` | Completion checkbox |
| `test-todo-tags` | Tags container |
| `test-todo-tag-work` | Work tag |
| `test-todo-tag-urgent` | Urgent tag |
| `test-todo-edit-button` | Edit button |
| `test-todo-delete-button` | Delete button |

### Stage 1A Test IDs (New)
| Test ID | Element |
|---------|---------|
| `test-todo-edit-form` | Edit form container |
| `test-todo-edit-title-input` | Title input field |
| `test-todo-edit-description-input` | Description textarea |
| `test-todo-edit-priority-select` | Priority dropdown |
| `test-todo-edit-due-date-input` | Due date input |
| `test-todo-save-button` | Save button |
| `test-todo-cancel-button` | Cancel button |
| `test-todo-status-control` | Status dropdown |
| `test-todo-priority-indicator` | Visual priority indicator (colored dot) |
| `test-todo-expand-toggle` | Expand/collapse button |
| `test-todo-collapsible-section` | Collapsible description container |
| `test-todo-overdue-indicator` | Overdue badge |

## Visual State Changes

| State | Visual Effect |
|-------|---------------|
| **Done** | Strike-through title + muted colors |
| **High Priority** | Red left border + red dot |
| **Medium Priority** | Orange left border + orange dot |
| **Low Priority** | Green left border + green dot |
| **Overdue** | Red accent background + red badge |
| **In Progress** | Blue gradient background |

## Accessibility
- ✅ Meaningful ARIA labels on buttons and interactive elements
- ✅ `aria-live="polite"` for time remaining updates
- ✅ Visible focus outlines on all interactive elements
- ✅ Keyboard navigable (Tab, Enter, Space)
- ✅ Semantic HTML (`article`, `form`, `label`, `select`, `time`)
- ✅ Color contrast WCAG AA compliant
- ✅ Screen reader friendly

## Responsive Breakpoints
| Breakpoint | Behavior |
|------------|----------|
| Mobile (<480px) | Stacked layout, reduced padding |
| Tablet (481-768px) | Adjusted spacing |
| Desktop (>768px) | Full card width (max 560px) |

