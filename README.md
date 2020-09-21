# Assignment 2: Babylon.js and TypeScript

**Due: Monday, September 27, 10:00pm CDT**

Description. 

## Submission Information

You should fill out this information before submitting your assignment.  Make sure to document the name and source of any third party assets such as 3D models, textures, or any other content used that was not solely written by you.  Include sufficient detail for the instructor or TA to easily find them, such as asset store or download links.

Name: 

UMN Email:

Build URL:

Third Party Assets:

## Rubric

Graded out of 10 points.  Empty template project.  Each of the parts to be added are presented in lecture or covered in one of the lessons in the [Babylon 101](https://doc.babylonjs.com/babylon101/) tutorials.

1. Create an outdoor scene
2. Create N objects
3. Add multiple lights, ambient, directional, spotlight, pointlight
4. Add a skybox
5. Camera with collisions and gravity
6. Upload a working build

**Bonus Challenge:**  Make one of the mesh objects follow the player

## Submission

You will need to check out and submit the project through GitHub classroom.  The project folder should contain just the additions to the sample project that are needed to implement the project.  Do not add extra files, and do not remove the `.gitignore` file (we do not want the "node_modules" directory in your repository.)

**Do not change the names** of the existing files.  The TA needs to be able to test your program as follows:

1. cd into the directory and run ```npm install```
2. start a local web server and compile by running ```npm run start``` and pointing the browser at your ```index.html```

Please test that your submission meets these requirements.  For example, after you check in your final version of the assignment to GitHub, check it out again to a new directory and make sure everything builds and runs correctly.

Make sure to document all third party assets. ***Be aware that points will be deducted for using third party assets that are not properly documented.***

## Local Development 

After checking out the project, you need to initialize by pulling the dependencies with:

```
npm install
```

After that, you can compile and run a server with:

```
npm run start
```

Under the hood, we are using the `npx` command to both build the project (with webpack) and run a local http webserver on your machine.  The included ```package.json``` file is set up to do this automatically.  You do not have to run ```tsc``` to compile the .js files from the .ts files;  ```npx``` builds them on the fly as part of running webpack.

You can run the program by pointing your web browser at ```https://localhost:8080```.

## Build and Deployment

After you have finished the assignment, you can build a distribution version of your program with:

```
npm run build
```

This project also includes a `deploy.sh` script that can automate the process of copying your assets to the `dist` directory, deploying your build to the web server, and setting public permissions.  To use the script, you will need to use a Unix shell and have`rsync` installed.  If you are running Windows 10, then you can use the [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10).  Note that you will need to fill in the missing values in the script before it will work.

## License

Material for [CSCI 5619 Fall 2020](https://canvas.umn.edu/courses/194179) by [Evan Suma Rosenberg](https://illusioneering.umn.edu/) is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

The intent of choosing CC BY-NC-SA 4.0 is to allow individuals and instructors at non-profit entities to use this content.  This includes not-for-profit schools (K-12 and post-secondary). For-profit entities (or people creating courses for those sites) may not use this content without permission (this includes, but is not limited to, for-profit schools and universities and commercial education sites such as Coursera, Udacity, LinkedIn Learning, and other similar sites).   

## Acknowledgments

This assignment was based upon content from the [3D User Interfaces Fall 2020](https://github.blairmacintyre.me/3dui-class-f20) course by Blair MacIntyre.
