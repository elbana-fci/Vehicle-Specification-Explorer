# Vehicle Specification Explorer

## Open and edit
Open index.html in a modern browser. All authored CSS and JavaScript are readable and commented inside that file. There is no build step and no separate component CSS or JS file.

Keep the _shared folder and truck-image.jpg next to index.html. The package contains local Messina Sans and Suisse Works fonts, Bootstrap 4.6.1 CSS and Font Awesome 5.9.0 CSS/webfonts. Third-party minified files are the original supplied vendor assets; the component itself is not minified. Bootstrap's grid matches the reference demo container. Its JavaScript, Popper and jQuery are not needed by the native disclosure controls.

## Source guide
- Demo header: navy introduction bar and expandable implementation note, matching maintenance-repair-card.html.
- Styles: template fonts/header, scoped layout, navy/cyan palette with muted teal specification accents, mentor feedback and motion preferences.
- Markup: Overview navigation, hidden task panel, mentor portrait/message, vehicle disclosures, task launcher below the overview and Good Roads footer.
- Script: reference data, delayed mentor feedback, description lists, mode switching/relocation, click-only activation, hints and reset. Change mentorDelay (350 milliseconds, followed by a 400ms fade) to adjust the initial message delay.

## Interaction
Overview starts with all categories closed and Find a specification below the overview card. Only clicking the task button moves it next to Overview, shows the task panel above the vehicle, and scrolls smoothly to it. Scrolling into view never starts the task. The task-box highlight and Knowledge nugget label are removed. Keyboard users can activate the button.

The mentor message starts after 350 milliseconds and fades in over 400 milliseconds, completing within one second. Reduced motion skips the fade. Open a category and select a value. Wrong answers produce mentor guidance in a pale red container and scroll smoothly to the mentor; optional hints use the same panel. Correct selection highlights the answer and updates the mentor with: “Congrats! Correct. The engine type is 3.5L 6-Cyl. w/10 Speed Automatic. You found it in the Engine category.” Focus moves to the feedback with preventScroll, then the page scrolls smoothly to the mentor container. Reduced motion uses an immediate scroll. There is no confetti, award or audio. Restart closes categories and schedules new guidance; Overview returns the task button below the card. Pending mentor timers are cancelled so delayed guidance never overwrites success or hints.

mentor.svg is an editable, local vector illustration of a course mentor in a hard hat and safety vest.

## Accessibility and scope
Native buttons and details/summary support Tab and Enter/Space. Visible focus, semantic headings/lists, explicit text feedback and decorative hidden icons are provided. Focus moves to the task heading on entry/restart, and moves to the mentor feedback on success. Layout stacks at narrow widths. Without JavaScript, the vehicle overview remains but values and activity require JavaScript; a notice explains this. One component per page is supported.

## Data notes
Data comes from truck-info.jpeg, not an independent vehicle database. Ambiguous torque and corrosion fields retain the reference information without invented units or mileage. The blank range is a dash. The cropped Emissions heading has no readable values, so no values are fabricated.

## Checks
Passed: inline JavaScript syntax, unique HTML IDs, local asset/font references, icon names present in supplied Font Awesome, and reduced-motion guard checks. DOM-simulated checks also passed for task relocation, delayed feedback, wrong/right selections, exact success text, timer cancellation, restart, click-only activation and reduced-motion scrolling. Browser rendering, native keyboard behavior and screen-reader testing remain unverified because no browser executable is installed. Manually check mobile/tablet/desktop widths, 200% zoom, both modes, wrong/right answers, hints, restart, and reduced motion before submission.

No repository push or email was performed: no destination repository or recipient was supplied.

Specification value buttons have neutral grey borders until selected. Selected answers use navy, with green on correct answers. Genuine keyboard focus remains visible. All #260c79 occurrences were replaced with #192f7c.
