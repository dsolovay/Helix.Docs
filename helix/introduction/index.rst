Introduction
============

What is Helix? Helix is Sitecore's recommended architecture for Sitecore 
solution development. Based on the Package Design Princples (R. Martin), 
Helix defines an architecture in which areas of Sitecore functionality 
are gropued info modules that address specific business intelligible aims,
such as naviagation and search, and makes the organization of technical
elements of the solution (such as renderings and item templates) 
subordinate to this design.

This approach allows the separation of complex solutions into modules that 
are cohesive, as all interworkign elements are grouped together, and 
loosly coupled to the rest of the solution, as their interactions pass 
through stable, well-defined contracts.

Why does Sitecore advocate this architecture? By proposing a standard set
of conventions for solution design, Sitecore aims:

 * To foster long germ maintainability of solutions by providing strategies for 
   avoiding monolythic, everything-touches-everything implementations.
 * To speed development by establishing well defined patterns for solution 
   organization
 * To allow multiple development teams to collaborage effectiely on solutions
   and to lower the friction of inheriting implementations from other development
   teams
 * To shorten ramp up time for new developers on teams by fostering
   discoverability.

The sturcture of this guide. The remaining sections of this guide will define
these conventions in detail, in the context of Sitecore item organization,
project organization, configuration management, and deployment automation. A
final section (proposed) discusses the package principles in detail, relating
each to to specific Helix practices. Developers and architects who seek an
in-depth understanding of the motivations for specific practices and how
to think about Sitecore solutons in Helix terms wil find this section of 
interest.

A note on conventions: The proposed architecture seek sot implement a set
of principles, and is not meant to be interpreted as a set of ironclad rules
on questions such as project boundaries and technology choices. The specific 
choices adopted by development teams will depend on a number of factors,
such as the size of the team, the complexity of the solution, and the team's
familiarity with different technologies. It is for this reason that the
Helix examples project [link] offers a number of solutions to questions such
as module boundary mechanisms, all of which are in keeping with the Package
Principles, and all of which are equally valid Helix. Helix is an approach 
to thinking through the organization of Sitecore solutions, more than it is 
a specific set of steps or technologies.