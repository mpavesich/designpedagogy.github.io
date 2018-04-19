---
layout: page
title: Collaboration
tag: Collaborative
d3: true
---

Collaborative practices are foundational to design pedagogy. We found collaboration in design studio contexts to be implicit, an assumed structure for acting and learning. During our research, we identified three primary kinds of collaboration: 1) student-student collaboration, 2) student-faculty collaboration, and 3) student-jury/clients collaboration. 

As writing and rhetoric instructors, student-student collaboration was the most familiar to us. The students we observed worked in teams and often performed peer assessment. 
https://drive.google.com/file/d/0B-Xz5YEzHzWEQnFoTk1KZjFGYWc/view (17)
However, this kind of peer work went well beyond a single project or activity. Frequently, teams of students work together on multiple projects throughout the semester. In some cases, student collaborations span across time, continuing from one semester to the next. For example, as Martin, a student from the LEED Lab, explained to us in this interview clip, https://drive.google.com/file/d/0B-Xz5YEzHzWEbVd1aTl4SjVqb1E/view (47) a student team might continue to work on the same or another student team’s project from a previous semester. The coordination of learning, in this instance, extends across space and time.  

In terms of student-faculty collaboration, the classes we attended presented a rigorous model of distributed authorship. Sometimes, for instance, instructors worked with students on particular aspects of their projects. While teachers continue to provide guidance and mentorship in student-faculty collaboration, they also contribute to projects in ways that may not be recognizable to most humanities faculty. The fact that professors are willing to step into the role of collaborator changes their relationship with students. As LEED lab student Joanna describes in this clip, students feel that there is a “mutual respect” that is carried throughout the semester, which changes the classroom dynamics. 
https://drive.google.com/file/d/0B-Xz5YEzHzWEcTFsVy1jQjVZTWs/view. (44) To cultivate this kind of working relationship, however, Joanna’s peer Martin adds that everyone— including professors—“checks their egos at the door.”
https://drive.google.com/file/d/0B-Xz5YEzHzWENmQxNC1JX09Dd28/view. (46)

In addition to peers and faculty, students also work directly with clients and jurors. In these situations, jurors are not merely critical evaluators, but often become collaborators, too. They push on and expand student ideas and offer new suggestions or possibilities.
https://drive.google.com/file/d/0B-Xz5YEzHzWEbktRbENEY3pVbktwaThUcnZGVlpKcmlQVTRZ/view?usp=sharing (83)
In this photo, jurors who are industry experts in architecture and urban planning circulate among student teams. During this critique, we observed jurors leaning in close, tracing lines with their figures, speaking familiarly with students, offering criticisms and possible solutions, and—in one notable instance—taking off a pair of high heels and stepping into model of a multi-block site in order to kneel down and point out a particular change that would enable smoother flow of delivery traffic.

Jurors also bring interdisciplinary perspectives that necessarily extend and complicate the student team’s knowledge base, as Joanna explains in this interview clip. 
https://drive.google.com/file/d/0B-Xz5YEzHzWEb1BFdFpzWFVQd1E/view (41)
In this sense, jurors serve as unofficial team members. Further, they sometimes have multiple points of interaction, since the same jury will often make more than one appearance in a semester. In addition, some clients, like the person shown in the wheelchair in the picture below, are essential collaborators. https://drive.google.com/file/d/0B289UM_oMdcRa3pqOUFQYm9FbGc/view (14) Without the input about this client’s needs and desires, as well as his physical embodied interactions with the prototypes, the student engineering team at UMBC would not have been able to design suitable enough equipment that would enable their client to thrive as a wheelchair lacrosse player. 

We want to acknowledge that these complex forms of collaboration are challenging, and they are sometimes met with resistance. For example, they require a lot of logistics that can be time consuming. Students also might worry about who their partners are and whether or not they will get stuck with an unfair amount of the work.
More broadly, as UMBC mechanical engineering professor Neil Rothman stated in our interview, students are not used to the kind of freedom and responsibility associated with “active learning.”
https://drive.google.com/file/d/0B-Xz5YEzHzWEeEtDRlJ1ZVlZUDQ/view (18)

One way that Georgetown’s Studio Collaborative responded to student concerns about collaboration was through a peer and self assessment tool. Articulated as part of the overall grading strategy, included in this document as well, students were asked to reflect on their own and their teammates’ contributions to the project.
	https://drive.google.com/file/d/0B-Xz5YEzHzWET1lPQkRJM1VBRjQ/view (73)
This additional writing assignment, completed individually, allowed students to feel like faculty could take each of their voices into account—to avoid being completely subsumed into their team. From the faculty side, the peer and self assessment tool is simply another way of creating interaction, or to coordinate different experiences into possible learning.

Finding ways to overcome the challenges of collaboration is vital, a point that Cathy Davidson stresses throughout The New Education. Davidson writes that “institutions should foster deep, integrated learning . . . by cultivating the difficult and increasingly necessary skill of collaborating with those whose expertise and cultural background may be radically different from one’s own” (232). Because this kind of collaboration can be so complex, it is essential that students have opportunities to reflect on how collaboration works. For example, Rebecca, a Georgetown student, reflected on her collaborative path by illustrating this map—though of course it was not only her path, as her map makes quite clear.
https://drive.google.com/file/d/0B-Xz5YEzHzWEdkthTTh1YllfNHM/view (26)

Rebecca depicted her team’s collaborative work throughout one semester (one option for work in the peer and self assessment document included above) to better understand the various elements that made this collaboration effective. Consider, for example, as an instance of faculty-student collaboration, the notation for February 29 in which Rebecca includes a text exchange with her teammates about a conversation she had with the instructor of their rhetoric course. As an example of student-juror collaboration, note the email with a juror on April 14, a date that falls between midterm and final crits, where the juror suggests a particular model for the project. On a larger scale, Rebecca’s map demonstrates the ebbs and flows that occur when collaboration serves as the foundation of learning experiences. Again, this metacognitive assessment of collaboration is key to helping students gain knowledge about what successful (and unsuccessful) collaborative processes look like—knowledge that they can apply to future collaborative opportunities. 


<script type="text/javascript">
  var w = 960,
      h = 500;

  var vertices = d3.range(100).map(function(d) {
    return [Math.random() * w, Math.random() * h];
  });

  var svg = d3.select("#graphic")
    .append("svg:svg")
      .attr("width", w)
      .attr("height", h);
  var paths, points, clips;
  clips = svg.append("svg:g").attr("id", "point-clips");
  points = svg.append("svg:g").attr("id", "points");
  paths = svg.append("svg:g").attr("id", "point-paths");
  
  clips.selectAll("clipPath")
      .data(vertices)
    .enter().append("svg:clipPath")
      .attr("id", function(d, i) { return "clip-"+i;})
    .append("svg:circle")
      .attr('cx', function(d) { return d[0]; })
      .attr('cy', function(d) { return d[1]; })
      .attr('r', 20);

  paths.selectAll("path")
      .data(d3.geom.voronoi(vertices))
    .enter().append("svg:path")
      .attr("d", function(d) { return "M" + d.join(",") + "Z"; })
      .attr("id", function(d,i) { 
        return "path-"+i; })
      .attr("clip-path", function(d,i) { return "url(#clip-"+i+")"; })
      .style("fill", d3.rgb(250, 250, 250))
      .style('fill-opacity', 0.5)
      .style("stroke", d3.rgb(190,230,230));

  points.selectAll("circle")
      .data(vertices)
    .enter().append("svg:circle")
      .attr("id", function(d, i) { 
        return "point-"+i; })
      .attr("transform", function(d) { return "translate(" + d + ")"; })
      .attr("r", 2)
      .attr('stroke', 'none');

  </script>



