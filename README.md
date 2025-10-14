Anyone Can Cook Inc. HR Portal Management Guide
Welcome to the management guide for the Anyone Can Cook Inc. Single Page Application (SPA) HR Portal! This document explains how to update job listings and manage the content of the portal.

1. Project Overview and Key Files
This portal is a single HTML file (index.html) containing all the website structure, styling (Tailwind CSS), and data/logic (JavaScript). All open job listings are stored directly within a JavaScript array called JOB_DATA.

2. Managing Job Openings (The JOB_DATA Array)
All job content is managed by editing the JavaScript array named JOB_DATA. You can find this array inside the <script> tag near the top of the index.html file, under the comment <!-- Embedded Job Data (from jobs.json) -->.

A. How to Add a New Job Opening
To add a new job, insert a new JSON object (a section enclosed in {} and separated by commas) into the JOB_DATA array.

Copy a template: Copy the structure of an existing job object, starting from the opening curly brace { to the closing }.

Paste and populate: Paste the copied object as the next item in the array. Crucially, ensure you separate it from the previous job with a comma (,).

Update fields: Fill in the values for the new role:

id: Must be a unique number (increment the last one, e.g., if the last ID was 8, use 9).

title: The exact title of the role.

department: The hiring department.

location: Where the job is based.

poster: (Optional) The path to an associated image, e.g., "posters/new-role-image.jpg".

responsibilities and qualifications: Update the list of strings (bullet points) for these sections.

B. How to Remove a Job Opening
To remove an existing job opening, simply delete the entire JSON object corresponding to that job from the JOB_DATA array.

Locate the job object you wish to remove (e.g., the object starting with "id": 5).

Select the entire block of code, starting from the opening { and ending with the closing }.

Delete it. If the job you are removing is followed by another job, ensure you also remove the trailing comma (,) that separates it from the next entry. If the job you remove is the last one in the array, make sure there is no comma before the closing square bracket ].

3. Asset Management (Images)
For images to display correctly, you must ensure they are in the correct folders:

Brand Logos: Images for Purple Oven, Goffa, and Village Cook are all stored in the assets/img/ folder.

Job Posters: If you want to use the optional poster field in the job data, those images should be located in a folder named posters at the root of your project.

Ensure that the file names and extensions (e.g., .png, .jpg) match exactly what is written in the index.html file.
