# Media Viewer

A browser-based media viewer for local files with advanced features for viewing images, videos, audio, and documents.

## Description

Media Viewer is a single-page web application that allows you to browse and view local media files directly in your browser. It uses the File System Access API to access folders on your device, maintaining a history of recently accessed directories.

## Features

### Core Functionality
- Browse and view files from local directories
- Support for multiple file types:
  - Images (PNG, JPG, JPEG, etc.)
  - Videos (MP4, WebM, etc.)
  - Audio (MP3, WAV, etc.)
  - Documents (PDF, text files)
  - Basic preview for other file types

### Media Navigation
- Thumbnail-based queue system
- Drag-and-drop reordering of queue items
- Next/previous navigation
- Shuffle functionality

### Media Controls
- Play/pause for video and audio
- Time scrubbing with progress bar
- Duration display
- Auto-advance to next file when media ends

### Folder Management
- Recently opened folder history
- Pin/star important folders for quick access
- Add new files to current directory

### User Interface
- Dark theme interface
- Responsive design
- File thumbnails in queue
- Fullscreen mode
- Auto-hiding controls when viewing video

### Keyboard Shortcuts
- Left/Right arrows: Previous/next file
- Ctrl+Left/Ctrl+Right: Previous/next file (when media is playing)
- Left/Right arrows: Seek -10/+10 seconds (in video/audio)
- Space: Play/pause
- F: Toggle fullscreen
- Q: Toggle queue sidebar
- Escape: Exit fullscreen or close dialogs

## Technical Details

### Technologies Used
- HTML5
- CSS3
- JavaScript (vanilla)
- File System Access API
- IndexedDB for storing folder references
- LocalStorage for recent folder history

### Browser Compatibility
- Chrome
- Edge
- Other Chromium-based browsers with File System Access API
- Fallback for browsers without File System Access API

## Usage

### Getting Started
1. Open the application in a supported browser
2. Click the folder icon to select a directory
3. Navigate through files using the interface or keyboard shortcuts

### File Queue
- Click on the list icon to show the queue
- Drag and drop items to reorder
- Click on a file in the queue to view it
- Use the shuffle or sort buttons to reorganize

### Recent Folders
- Previously accessed folders appear on the start screen
- Star/pin important folders for quicker access
- Click on a folder to open it again
- Remove folders from history using the X button

### Adding Files
- Click the + button to add new files to the current directory
- Drag and drop files into the add file dialog
- Files are saved to the current directory if possible

## Implementation Notes

The application is implemented as a single HTML file with inline CSS and JavaScript. It uses modern JavaScript features and APIs, particularly:

- File System Access API for directory browsing
- IndexedDB for storing directory handles
- LocalStorage for recent folder history
- Drag and drop API for queue management
- Canvas API for video thumbnails
- Media elements for playback

For browsers without File System Access API support, a fallback mechanism allows selecting individual files instead of directories.
