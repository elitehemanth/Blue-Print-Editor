# Blue-Print-Editor
#  Description

This project is an offline, client-side Blueprint Editor.
It lets a user create draggable “nodes,” each containing multiple description rows, images, and interactive connection pins. Nodes can be linked using long-press gestures on pins, stored in JSON, restored later, and exported as images or PDF. The UI also supports undo/redo, zoom, and deletion tools.

Its purpose is to visually map workflows, ideas, system architecture, class diagrams, or planning structures without needing a backend.

# Key Features
Node system

Create unlimited description nodes.

Each node contains:

Editable title

Editable description rows

“Add row” and “Delete selected row” actions

Image attachment inside any description row

Draggable movement (with handle)

Linking system

Long-press a left or right pin to start a link.

Drag to another pin to create a curved connection.

Automatically redraw connections when nodes move.

Undo-safe.

Zoom & Navigation

Smooth canvas zoom (buttons or Ctrl+scroll)

Centered zoom based on click location

Large fixed canvas (2000×1400px)

Undo / Redo

Full state snapshot system

Up to 80 historical states

Save / Load

Save blueprint to .json

Load .json back to restore entire layout

Exporting

Export entire canvas as:

High-res JPG/PNG

PDF (through html2canvas + jsPDF)

UI Toolbar

Add node

Add image to selected row

Undo / Redo

Clear canvas

Delete selected node

Export (Image / PDF)

Save / Load JSON

# Requirements
Dependencies

The HTML file loads two libraries (bundled locally):

html2canvas.min.js — for exporting the canvas as an image

jspdf.umd.min.js — for PDF generation

Browser

Any modern browser supporting:

ContentEditable

Pointer events

Flexbox & transforms

SVG paths

Local file input (for JSON load)

No server required.

# How to Use the Editor
1. Creating Nodes

Click “+ Description Node”.
A new node appears with:

Title

One default description row

Add/Delete row buttons

Drag handle

Click anywhere in the node to select it.

2. Adding Descriptions

Inside a node:

Click “+ Desc” to add new editable rows.

Click a row to select it.

Use Delete key or the Delete Row button to remove that row.

3. Adding Images

Select a row.

Click “+ Add Image to Selected”.

Paste an image URL.

Images embed inside the row and resize automatically.

4. Moving Nodes

Drag the blue circular handle in the bottom-right corner.

Connections update automatically.

5. Linking Nodes

Long-press (200ms) on a pin (blue arrow on left or right side of row).

Drag cursor.

Release over another pin.

A curved SVG line appears linking both rows.

6. Zooming

Use + / − buttons at bottom-right.

Or hold Ctrl + scroll.

Click anywhere to set zoom anchor point.

7. Saving Work

Click “Save .json”.
A JSON file downloads containing:

All nodes

Titles

Rows

Images

Connections

Positions

8. Loading Work

Click “Load .json” and select a previously saved file.

The entire layout is restored.

9. Exporting

Export as Image → PNG/JPG of the entire canvas

Export as PDF → PDF centered on page

Useful for reports or presentations.

#  Use Cases
 System Architecture

Map server-client designs, APIs, microservices, or data flows.

Software Planning

Outline module interactions, dependencies, and logic flows.

Business Workflows

Visualize processes, decisions, or customer journeys.

#Game Design

Quest trees, dialogue trees, level flow planning.

Education / Learning

Mind maps, visual study notes, flow explanations.

#Brainstorming

Capture ideas with flexible visual structure.

# Buttons Purpose
<hr>
<img width="1611" height="954" alt="Screenshot 2025-11-30 222655" src="https://github.com/user-attachments/assets/07cd910b-144d-43fb-8ba2-475fd08a9c46" />
<hr>

# Example Use Case
<img width="1619" height="951" alt="Screenshot 2025-11-30 221337" src="https://github.com/user-attachments/assets/35f09a71-43c2-4d47-8f7a-07d3d258ab67" />
<hr>


# Not My Style
