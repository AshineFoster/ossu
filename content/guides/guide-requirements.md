+++
title = "Syllabus Guide Requirements"
weight = 1
+++

Background:
Some students have voiced concerns that the course material is not convenient to access and/or doesn't tell the full story of how to complete the course. A few examples:

In the beginning course of the program, Python for Everybody, OSSU links to the course creator's Py4E homepage, which contains links to several different versions of the course. People are commonly confused as to which version of the course should be chosen, how to get started, and why some versions are asking for money when OSSU is supposed to be free. There exists insider knowledge stating that the course should be taken directly on py4e.com, but this is not communicated unless people ask in the Discord channel.

In another early course, How To Code, OSSU links directly to an EdX enrollment landing page which asks for payment to go Verified. The course paywalls a portion of the course content, confusing people into believing that they are missing out on a substantial portion of the course. There exists insider knowledge stating that the paywalled content can be ignored safely, but this is not communicated unless people ask in the Discord channel.

In a core course, Operating Systems - Three Easy Pieces (OSTEP), OSSU links to the course creator's course homepage. While informative, this page is not easy to navigate, and it is easy for people to miss the step-by-step list of assignments and the supporting material which assists with those assignments. Further, at least one unofficial source links to the course creator's textbook homepage, which resides at the same website and is easy to mistake for the course homepage. It is less easy to navigate, and confusingly contains some (but not all) of the material for the course.

In each of these circumstances, completion of the courses is made more difficult due to lack of information about how to use the materials available. Such problems could be mitigated by the development of a course README or syllabus for each class in the OSSU curriculum.

Some of this is currently mitigated by the existence of the OSSU Discord, and indeed the individual Discord course channels hold pinned posts conveying much of this information. However, in my view we should not assume that:

-   all OSSU curriculum users are on the OSSU Discord,
-  all OSSU Discord users are aware of information in the pinned posts, or
-    the subset of OSSU Discord users that are aware of pinned posts are actively checking the pinned posts for information crucial to the successful completion of the course.

Further, there is precedent around the notion that the OSSU Github page should be the one, true official repository of OSSU course information. For that to be the case, in-group knowledge gained by current students should be communicated to the community-at-large via the official channels. This enables those official channels to stand alone.

The OSSU curriculum page provides high-level information about every course in the curriculum, similar to a university's course catalog. It is probably not the appropriate place to communicate a lot of course-specific information.

The solution I am proposing involves creating a place for OSSU to communicate course-specific information, similar to a university's course syllabus. The OSSU curriculum page could then link to the syllabus for each course. Such a page could also be considered a README for the course.

Advantages would include:

- It provides a central location to contain and maintain course information.

- It standardizes the course - allowing students to know exactly what work must be completed to finish the course, and where to find all the relevant resources.

- It can improve student experience, positively impacting student outcomes and program retention.

- It provides for the archival and persistence of inside information. As students complete a course, they tend to hang around the Discord for a few weeks, then either leave OSSU entirely or concentrate their attention on another course. In either instance they take their valuable inside information with them. In popular courses some of this knowledge is perpetuated; in many later courses with few users, much of this inside information is likely lost until rediscovered by another student.

- It provides consistency of information, so that the information provided to anybody who asks represents the best information known to all in OSSU.

Potential disadvantages would include:

    The mere existence of a syllabus/README does not guarantee that people will willingly use it. We can mitigate this by making the pages a) lean, b) useful, and c) easy to navigate. Once they are developed, we can reconfigure the OSSU course page to link to the README instead of directly to the course, ensuring that all new users at least see it once.
    This will permanently increase the amount of development and maintenance time on the curriculum as a whole. Approximately 30 README pages will need to be created and maintained. We should crowd-source this effort by creating a standard template and encouraging people to make PRs during and after their time in the courses.

Proposal:
Provide a README file comprising a course syllabus for each course in the OSSU curriculum.

In order to maximize added value, each syllabus should prioritize, in the following order:

    leanness -- the syllabus should contain only the information needed to aid in course completion, with only minimum narrative. Instructions should be terse and easy to follow -- "go here, do this".
    usefulness -- the syllabus should contain all of the information needed to succeed in the course, along with any supporting documentation or alternate sources.
    ease of navigation -- course material should be laid out in a linear, easy-to-follow manner. Lists and tables should be utilized wherever appropriate.

The syllabus should include the following information at a minimum:

    A statement of course objectives, to provide motivation for completing the course. This should be no longer than 2 sentences.
    A statement of course outcomes, or a listing of the specific competencies in CS2013 the course is thought to cover/satisfy.
    A list of immediate prerequisites and a statement of the expected duration of effort.
    A Getting Started section, which shall contain:
        A link to the website, "start" page, or lander where the course resides.
        "Turn-by-turn" directions for new student onboarding: choosing which section of the course to sign up for, how to sign up, whether or not payment information is required, and anything else required to enroll.
        Include any assurances that the complete course is available for free, or any time durations users should understand before starting ("free access expires in 6 weeks, so don't sign up until you're ready to work", etc.)
        A short list of 1-2 alternate locations for accessing course content (if applicable) with a clear statement that these locations are OPTIONAL.
    A Course Materials section, which shall contain either:
        A link to the Course Materials page of the course website, or
        A list of all lessons in the course, with a link to each individual lesson or the beginning of each chapter/section.
        Also, a list of any Supplementary Materials (course videos, recitation sections, optional lectures, etc.) This could include a short, 1-line note motivating why a student may want to use these supplements ("recitation videos provide guided homework practice!", etc.)
    An Assignments section, which shall contain either:
        A link to the Assignments page of the course website, or
        A list of all assignments in the course, with a link to each individual assignment.
    (Stretch Goal) A Roadmap To Completion checklist section, which could optionally replace the lessons list in "Course Materials" and the assignment list in "Assignments". It may look like:
        "Perform the steps in Getting Started"
        "View and take notes on Lessons 1.1-1.4"
        "Complete Homework 1, located --here--, as discussed in --this-- recitation video"
        "View and take notes on Lessons 2.1-2.5"
        etc.
        "Complete Final Exam and submit for approval"

Alternatives:

    Keep the status quo. This alternative involves the least effort in the short-term, but students will continue to experience the highest level of confusion while using OSSU course materials.
    Expand the OSSU curriculum page to contain a subset of this information. I feel this is the worst option because the curriculum page serves as a course catalog, and it is already monolithic. Further, it is the official "landing page" for new users of the program. Adding more information on this page would likely make this page even less useful.
