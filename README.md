# TimeLineSlider 📅  

A fully customizable, draggable timeline component for your web applications. You can set a range of years, customize the step intervals, and highlight special milestones. TimeLineSlider makes creating interactive timelines easy and beautiful.

---

## Features 🌟
- **Set a range of years**: Define the start and end years for your timeline.  
- **Customizable steps**: Specify step intervals between years.  
- **Special milestones**: Highlight specific intervals with unique styles.  
- **Draggable slider**: Drag and snap to specific years with smooth animations.  
- **Dynamic Active Year**: Active year automatically updates as you interact with the timeline.

---

## Installation 🛠️

Install the package via NPM:
     npm install timeline-slider  

## usage📖
Import and Initialize
Include the CSS (either manually or dynamically):

### Manual Import:
Add the CSS file in your HTML or import it in your JS:

    import 'timeline-slider/css';

Or:

    <link rel="stylesheet" href="node_modules/timeline-slider/css/main.css">

Import and use the TimeLineSlider class:

import TimeLineSlider from 'timeline-slider';

**there are defult values but there is an example:**

    const timeLineSlider = new TimeLineSlider();
    timeLineSlider.setStartEnd(1950, 2020); 
    timeLineSlider.setStep(1);             
    timeLineSlider.setSpecialStep(10);

## API Reference 🚀
- **setStartEnd(startYear, endYear)**
Defines the start and end years for the timeline.
Example:


      timeLineSlider.setStartEnd(1900, 2023);

- **setStep(step)**
Sets the interval between years on the timeline.
Example:

      timeLineSlider.setStep(5);

- **setSpecialStep(specialStep)**
Highlights specific years based on a custom interval.
Example:

      timeLineSlider.setSpecialStep(10); 

- **setActiveSlideClass(className)**
Sets the CSS class for the active year.
Example:

      timeLineSlider.setActiveSlideClass('active');

## Html 
### You should add an atribute "slide-year" to you slides or list like this: 
    <div slide-year="1998">
        <h1>
            1998
        </h1>
    </div>

## Styling  🎨
Customize the appearance of the timeline using the provided CSS classes:

### Key Classes:
- .one-line :- Regular timeline markers.
- .specifline:- Highlighted markers for special steps.
- .actor:- your custom activeSlideClass - The currently selected year marker.

Modify these styles in main.css to match your design.
