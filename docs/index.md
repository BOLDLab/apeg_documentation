<style>
.sqrt {
  vertical-align: middle;
  text-align: left;
  display: block;
  width: 600px;
}
.fraction {
  vertical-align: middle;
  text-align: center;
  font-size: 9pt;
}
.fraction > span {
  padding-top: 0.15em;
}
.fdn {border-top: thin solid black; }
.fraction > .bar {display: none}
.radical {
    font-size: 3.4em;
    display: inline-block;
    font-weight: 100;
}
.radicand {
    padding: 0.25em 0.25em;
    border-top: thin black solid;
    margin: 0em -2px 2.6ex;
    width: 17em;
    display: inline-block;
}
.ls {
    vertical-align: middle;
    margin-top: -25px;
    margin-right: 12px;
    font-size: 1.6em;
    font-weight: 100;
    display: inline-block;
}
#sapa .fdn {
  display: inline-block;
  width: 288px;
}
#sapa .radicand {
    width: 20em;
}
.ntm {
  width: 17em;
  display: inline-block;
}
.tms {
  font-size: 10pt;
  height: 3em;
  display: inline-block;
  vertical-align: middle;
  padding-right: 2em;
}
.fracti {
  display: inline-block;
  padding: 0.5em;
}
.acronym {
  font-size: 1.3em; font-weight: bold;
}
</style>

# APEG

APEG is a web application that allows students completing group work to evaluate each other's contribution to the group.

<span class='acronym'>A</span>__daptable__

APEG is HTML template driven via the [ExpressionEngine CMS](https://expressionengine.com/) and built on open-source software [libraries](https://github.com/BOLDLab/lti_peer_assessment), templates can easily be modified to provide custom content.

<span class='acronym'>P</span>__eer__ <span class='acronym'>E</span>__valuation__

Peer evaluation is the assessment or review of work by one or more people of similar competence to the producers of the work ([peers](https://en.wiktionary.org/wiki/peer#Etymology_2)) ([Wikipedia definition](https://en.wikipedia.org/wiki/Peer_review)).  

__for__    <span class='acronym'>G</span>__roups__

Groups of students are able to assess each others' contribution to a team using APEG.

APEG can incorporate a Blackboard&trade; [rubric](https://en.wikipedia.org/wiki/Rubric_(academic)) or allow students to supply a numeric 'grade' with comments. The application is optimised for use with the [Blackboard Learn&trade; VLE](http://anz.blackboard.com/sites/international/globalmaster/).

The application can be adapted to to any VLE that implements the IMS Global<sup>&reg;</sup> Learning Tools Interoperability<sup>&reg;</sup> (LTI) standard.  

## Peer Assessment Equations ##

APEG can be used in different modes, currently there is a simple 'mean' mode and an advanced SPA (Self Performance Assessment) mode.

#### <u>Mean Mode</u> ####
In the mean mode, each team member is given the average score they received from the group.

__When to use mean mode__
Mean mode is best if students are just required to grade each other's work performance in the team without any self-assessment.

<div class='sqrt'>
<span class='tms'>Individual Team Member's score </span><span class="radical tms"> =</span>
<div class='fracti'>
<span class='fraction'>Total ratings for individual team member <span class='bar'>&frasl;</span><br>
<span class='fdn ntm'>Number of team members</span>
</div>
</div>

#### <u>SPA Mode</u> ####
The SPA mode compares the each team members' self assessment against the rating given by the rest of the group.
SPA mode is best

This mode uses equations developed by [Willey, Freeman and Gardner (2010)](http://www.tandfonline.com/doi/full/10.1080/03043797.2010.490577?scroll=top&needAccess=true) at UTS, Sydney, Australia.

__When to use SPA mode__

SPA mode is best used when the instructor would like to give students a group mark for an artefact they have produced. The SPA score generated is then used as a multiplier of the group mark for each individual in the group. High and low contributors to group work are therefore awarded according to their perceived group contribution.

__Details__

The SPA mode provides a multiplier for instructors to apply to group work scores and a Self Assessment to Peer Assessment (SAPA) factor as a feedback score to students.

A SPA score equal to or greater than 1.0 indicates the student contributed the maximum amount possible, based on the rest of the group's ratings, to the group work.  

A SPA score less than 1.0 indicates that the student contributed under the maximum amount possible to contribute, based on the rest of the group's ratings, to the group work.

So if the group project scored an 89 and Waleed scored a SPA of 0.83, Waleed would receive 89 * 0.83 = 74 (rounded up from 73.87).

<div class='sqrt'>
<span class='ls'>SPA =</span> <span class='radical'>&radic;</span><div class='radicand'><span class='fraction'>  Total ratings for individual team member <span class='bar'>&frasl;</span>
<span class='fdn'>Average of total ratings for all team members</span></span>
</div>
</div>

The SAPA gives students an indicator of how they perceive their own performance in relation to the group's perception of their performance.

<div class='sqrt' id='sapa'>
<span class='ls'>SAPA =</span> <span class='radical'>&radic;</span><div class='radicand' ><span class='fraction'> Self ratings for individual team member <span class='bar'>&frasl;</span>
<span class='fdn'>Average of ratings for individual by peer team members</span></span>
</div>
</div>

A SAPA score greater than 1.0 indicates students over-rated their performance in comparison to the group.  

A SAPA score less than 1.0 indicates students under-rated their performance in comparison to the group.

For further information on these equations please see the [Spark<sup>PLUS</sup> documentation](http://sparkplus.com.au/factors/).   

## [Students](guides/Students)
Assessing your group's members using the peer review platform

## [Instructors](guides/Instructors)
How to check student access, download grades and setup preferences.

## [Course Builders](guides/Course-Builders)
How to add the LTI link to your Blackboard Course
