---
layout: page
title: DIY Learning
tag: DIY
d3: true
---

Self-propelled learning is one of the most crucial aspects of design studio pedagogy. DIY (do-it-yourself) approaches to teaching encourage students to become responsible for their own learning. Arjun Dhillon, then-head of studio for the EthicsLab at Georgetown, describes DIY learning as a “squiggle.” In the drawing and audio field note below, which we recommend you listen to and look at simultaneously, Dhillon provides a sense of design work as requiring self-motivation and resilience—of knowing that you need to put in the work, and imagining the necessary steps as emerging from the end goals, rather than proceeding through the stages of a scaffolded assignment.  

Squiggle image [use image here not icon]: https://drive.google.com/file/d/0B-Xz5YEzHzWEYUJkbmktSmg0c00/view?usp=sharing (13)
Audio field note: https://drive.google.com/file/d/0B-Xz5YEzHzWERWVGbXBaelYwQ2M/view?usp=sharing (48)

DIY approaches often raise questions about students’ abilities, as novices, to work on their own. However, it is important to recognize that students are not starting from scratch or only working on their own. DIY approaches rely on the fact that students have already acquired what Jenny Rice calls “para-expertise.” Rice defines “para-expertise” as “the experiential, embodied, tacit knowledge that does not translate into the vocabulary or skills of disciplinary expertise” (119). DIY depends on the knowledge students have accumulated from lived experiences and encourages them to leverage or articulate that knowledge—to put it into practice. In other words, “para-expertise” is the engine of DIY; it is the reason why DIY approaches can work. All students bring prior learning, life experiences, and unique skills to any new situation. The sum total of students’ prior knowledge, experience, and skills commingles with the new disciplinary knowledge of a class, as well as the affordances and constraints of particular design challenges and interactions with teammates, faculty, and jurors.

In the studios we observed, students experienced DIY primarily through experimentation and productive failure. Additionally, students themselves determine to a great degree how they move between these experiences. We want to stress that DIY learning is not only about students conducting conceptual research or fact-finding missions on their own. Rather, it is an embodied practice in which students tinker with materials—in both digital and analog contexts—in order to try out different possibilities for their projects. In other words, as Dhillon puts it, the work of design is not always abstract:  https://drive.google.com/file/d/0BwBBuU_uLSSKczVmTm56UEVVNzA/view (12)

And when an idea or prototype fails during the experimentation process, students learn what does not work in order to get closer to what does work (hence, productive failure). Students often struggle, at least at first, with embracing failure in this way. For instance, Rothman elaborates on his students’ emotional reaction to their failure during the process of creating a prototype: 

https://drive.google.com/file/d/0B-Xz5YEzHzWEbGdPU1E0TlJXR3c/view (63)

Over time, however, students can become accustomed to and even appreciate failure in design studio models. Here is LEEDlab student Joanna on her experiences with failure: https://drive.google.com/file/d/0B-Xz5YEzHzWELU96MUZUQnFoU0k/view (45)

We find Joanna’s response particularly instructive. She describes the designer’s failure as requiring two kinds of responses, both of which we began to think of in terms of DIY: acquiring new knowledge for improving prototypes and the affective resilience to keep trying. As Dhillon puts it in this clip, “we don’t move them through it, they have to move through it themselves,” while describing the still-crucial but circumscribed role of scaffolding:
https://drive.google.com/file/d/0BwBBuU_uLSSKdElHVkxzUG5ibXc/view (7)

We also want to point out that while students’ independence is central to DIY learning, the teacher is not absent from this approach. Instead of providing constant direction and authority, however, the role of the teacher is to guide from a distance and collaborate, to zoom in and back out depending on the moment. Teachers often point students to resources or research, or check in on the progress of developing projects without telling students the “right” way to do things—in part because the right way to complete these projects does not yet exist in the world, if it ever could. Here are Martin and Joanna discussing how this sometimes frustrating method of teaching (from their point of view) forces students to become resourceful. https://drive.google.com/file/d/0BwBBuU_uLSSKT2lhaW1EbEowSUU/view (37)

Students are also expected to give reasons for why they make particular decisions. But as Martin and Joanna explain, that can be a difficult task when the community of respondents broadens through crits. Students/designers have to do-it-themselves in part because jurors rarely if ever agree on the best path forward, and students have to make a choice about how to proceed with the project in order for it to continue. Operating among a community of emerging practitioners and current experts means navigating dissent, making one’s own choices, and having reasons for those choices, as Joanna and Martin describe here:https://drive.google.com/file/d/0B-Xz5YEzHzWEUGxnZE1XUGI3Zlk/view (42)

We want to be clear that DIY does not diminish the value of expert knowledge; if anything, we observed the opposite in every studio we entered. The value of expert knowledge only seems to be heightened by designers working on projects that are collaborative, high impact, DIY, and ecological. Sometimes expert knowledge emerges in mini-lectures or just-in-time instruction, and sometimes it appears in the form of a teacher’s ability to design effective learning environments and experiences. This is something Rothman emphasized in our interview with him, when he distinguished between “teaching” and what we might call “facilitating learning”:  
https://drive.google.com/file/d/0B-Xz5YEzHzWEcTd4U0pYc2c0ZXM/view (15)

DIY approaches, then, offer something more akin to an apprenticeship in which teachers design guided opportunities for students to learn on their own through prior and new forms of knowledge. Incorporating DIY approaches into our pedagogies is especially important right now considering that technologies have transformed our everyday lives, including the workforce that students will be entering after college. In The New Education, Cathy Davidson repeatedly emphasizes that a focus on “learning how to learn” is “the single most important skill anyone can master” (14). She writes, “Learning how to learn equips students to become independent and demanding researchers who can use an array of creative, critical, and computational methods to solve problems, wherever they face them” (14-15). In all of the design studio settings we observed, students recognized the value of DIY practices in both their individual and collaborative learning processes; indeed, their individual success, and the potential impact of their work in the world, depended on such recognition.


<script type="text/javascript">
(function() {
    var paper, circs, i, nowX, nowY, timer, props = {}, toggler = 0, elie, dx, dy, rad, cur, opa;
    // Returns a random integer between min and max
    // Using Math.round() will give you a non-uniform distribution!
    function ran(min, max)
    {
        return Math.floor(Math.random() * (max - min + 1)) + min;
    }

    function moveIt()
    {
        for(i = 0; i < circs.length; ++i)
        {
              // Reset when time is at zero
            if (! circs[i].time)
            {
                circs[i].time  = ran(30, 100);
                circs[i].deg   = ran(-179, 180);
                circs[i].vel   = ran(1, 5);
                circs[i].curve = ran(0, 1);
                circs[i].fade  = ran(0, 1);
                circs[i].grow  = ran(-2, 2);
            }
                // Get position
            nowX = circs[i].attr("cx");
            nowY = circs[i].attr("cy");
               // Calc movement
            dx = circs[i].vel * Math.cos(circs[i].deg * Math.PI/180);
            dy = circs[i].vel * Math.sin(circs[i].deg * Math.PI/180);
                // Calc new position
            nowX += dx;
            nowY += dy;
                // Calc wrap around
            if (nowX < 0) nowX = 490 + nowX;
            else          nowX = nowX % 490;
            if (nowY < 0) nowY = 490 + nowY;
            else          nowY = nowY % 490;

                // Render moved particle
            circs[i].attr({cx: nowX, cy: nowY});

                // Calc growth
            rad = circs[i].attr("r");
            if (circs[i].grow > 0) circs[i].attr("r", Math.min(30, rad +  .1));
            else                   circs[i].attr("r", Math.max(10,  rad -  .1));

                // Calc curve
            if (circs[i].curve > 0) circs[i].deg = circs[i].deg + 2;
            else                    circs[i].deg = circs[i].deg - 2;

                // Calc opacity
            opa = circs[i].attr("fill-opacity");
            if (circs[i].fade > 0) {
                circs[i].attr("fill-opacity", Math.max(.3, opa -  .01));
                circs[i].attr("stroke-opacity", Math.max(.3, opa -  .01)); }
            else {
                circs[i].attr("fill-opacity", Math.min(1, opa +  .01));
                circs[i].attr("stroke-opacity", Math.min(1, opa +  .01)); }

            // Progress timer for particle
            circs[i].time = circs[i].time - 1;

                // Calc damping
            if (circs[i].vel < 1) circs[i].time = 0;
            else circs[i].vel = circs[i].vel - .05;

        }
        timer = setTimeout(moveIt, 60);
    }

    window.onload = function () {
        paper = Raphael("graphic", 1000, 1000);
        circs = paper.set();
        for (i = 0; i < 30; ++i)
        {
            opa = ran(3,10)/10;
            circs.push(paper.circle(ran(0,1000), ran(0,1000), ran(10,30)).attr({"fill-opacity": opa,
                                                                           "stroke-opacity": opa}));
        }
        circs.attr({fill: "#00DDAA", stroke: "#00DDAA"});
        moveIt();
        elie = document.getElementById("toggle");
        elie.onclick = function() {
            (toggler++ % 2) ? (function(){
                    moveIt();
                    elie.value = " Stop ";
                }()) : (function(){
                    clearTimeout(timer);
                    elie.value = " Start ";
                }());
        }
    };
}());
</script>
