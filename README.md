<img src="\images\💻CM20219.png"
     alt="Markdown Monster icon"
     style="float: left; margin-right: 10px;" />
# WebGL Coursework
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/choobs1/choobs1)

_Learning about 3D models using WebGL_

**Description:** The project demonstrates the various fundamentals of 3D modelling.
The user is allowed to use a few functionalities, thus providing an interactive experience.
## Installation
After going to the project directory the user may start a python server using the command line:
```
python -m http.server
```
It will tell the user on which port the server is listening to (by default:8000).
In your web browser, go to “http://localhost:PORT”, where “PORT” is the number reported earlier.

You may boot up the HTML file directly but the texture loading and the object loader will not work.

## Usage
```
function handleKeyDown(event) {
			switch (event.key) {				
				case 'f': // f = face
					//alert('TASK: add code for face render mode (requirement 4).');
					...

				case 'e': // e = edge
					//alert('TASK: add code for edge render mode (requirement 4).');
					...

				case 'v': // v = vertex
					//alert('TASK: add code for vertex render mode (requirement 4).');
					...
				/*
				*	TASK: add code for starting/stopping rotations (requirement 3).
				*/
				case 'g':
					//For starting rotations.
					...
				
				case 'h':
					//For stopping roations.
					...
			}

			/*
			* TASK: Implement code to help with translating the camera.(Requirement 5).
			*/
			switch(event.keyCode){
				case 37: // left arrow = translate camera left
                    ...

                case 39: // right arrow = translate camera right
                    ...
                       
				case 40: // down arrow = translate camera down
					...

				case 38: // up arrow = translate camera up
					...

				case 16: // left shift = translate camera forwards
					if (cameraZ != -0.01) {
						cameraZ = -0.01;
					}
					else {
						cameraZ = 0;
					}
					break;

				case 17: // left control = translate camera backwards
					...

				/*
				* TASK: Orbitting the camera in different directions(Requirement 6).
				*/	
				case 65: // a = orbit the camera left
                        ...

                case 68: // d = orbit the camera right
                        ...

                case 87: // w = orbit the camera upwards
                        ...

                case 83: // s = orbit the camera downwards
                        ...
			}
		}
        ```
        