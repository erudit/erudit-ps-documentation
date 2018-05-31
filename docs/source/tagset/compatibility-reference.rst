.. _compatibility-reference:

Compatibility Reference
=======================

This section have some tables for compatibility reference between :term:`Érudit Article` and :term:`Érudit PS`. 


@publication-type in :ref:`element-element-citation`
----------------------------------------------------

+-----------+-----------------+-------------------------------------------------------------------+
| Érudit PS | Érudit Article  |  Description                                                      |
+===========+=================+===================================================================+
| book      | livre           |  Refers to books. It can also represent only a part or chapter of |
|           |                 |  a book.                                                          |
+-----------+-----------------+-------------------------------------------------------------------+
| chapter   | livre           |  Refers to books. It can also represent only a part or chapter of |
|           |                 |  a book.                                                          |
+-----------+-----------------+-------------------------------------------------------------------+
| confproc  | actes           |  Identifies documents related to scientific events: minutes,      |
|           |                 |  annals, results, proceedings, conventions and conferences,       |
|           |                 |  among others.                                                    |
+-----------+-----------------+-------------------------------------------------------------------+
| data      | bd              |  Specifies databases.                                             |
+-----------+-----------------+-------------------------------------------------------------------+
| magazine  | armag           |  Refers to citations for non ccientific journals                  |
|           |                 |                                                                   |
+-----------+-----------------+-------------------------------------------------------------------+
| journal   | arrevue         |  Characterized by serial publications, edited in successive       |
|           |                 |  units / issues, with numerical and / or chronological            |
|           |                 |  designations, and destined to be continued indefinitely.         |
+-----------+-----------------+-------------------------------------------------------------------+
| patent    |                 |  Refers to patents.                                               |
+-----------+-----------------+-------------------------------------------------------------------+
| report    | rapport         |  Identifies a unique technical report, normally authored by an    |
|           |                 |  institution.                                                     |
+-----------+-----------------+-------------------------------------------------------------------+
| software  | logiciel,       |  Refers to a software distributed on CDs, DVDs, online media, USB |
|           | multimedia      |  devices, etc.                                                    |
+-----------+-----------------+-------------------------------------------------------------------+
| thesis    | these           |  Characterized by monographs, dissertations or theses to attain an|
|           |                 |  academic degree (doctorate, master's, baccalaureate, bachelor's  |
|           |                 |  degree, etc.).                                                   |
+-----------+-----------------+-------------------------------------------------------------------+
| webpage   |                 |  Identifies web sites e blogs.                                    |
+-----------+-----------------+-------------------------------------------------------------------+
| newspaper | arjournal       |  Identifies newspapers articles.                                  |
+-----------+-----------------+-------------------------------------------------------------------+

Values without correlation in Érudit PS:

    * art (Œuvre d'art)
    * audience (Audience)
    * audiovisuel (Documentation audiovisuelle)
    * autre (Autre type de référence bibliographique)
    * brevet (Brevet d'invention)
    * carte (Carte ou plan)
    * classique (Œuvre classique)
    * collectif (Ouvrage collectif)
    * comm (Communication)
    * commperso (Communication personnelle de l’auteur)
    * equation (Équation)
    * figure (Figure)
    * film (Film ou émission radiophonique ou télévisuelle)
    * gouv (Publication gouvernementale)
    * jurisprudence (Jurisprudence)
    * legislation (Législation)
    * manuscrit (Manuscrit)
    * nonpub (Ouvrage non publié)
    * partielivre (Partie d’un livre)
    * prepub (Prépublication)
    * projetloi (Projet de loi)
    * reglementation (Règlementation)
    * tableau (Diagramme ou tableau)

@abstract-type in :ref:`element-abstract`
-----------------------------------------

+-------------------+-------------------+-------------------------------------------------------------------+
| Érudit PS         | Érudit Article    |  Description                                                      |
+===================+===================+===================================================================+
| ASCII             | autre             |  A “plain text” abstract, i.e., without special characters or     |
|                   |                   |  equations, so the abstract can be sent in email or displayed on  |
|                   |                   |  primitive browsersRefers to books. It can also represent only a  |
|                   |                   |  part or chapter of                                               |
+-------------------+-------------------+-------------------------------------------------------------------+
| executive-summary | autre             |  A non-technical summation of the major findings of the article   |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| graphical         | autre             |  A pictorial representation such as a picture or a video          |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| editor            | autre             |  An abstract written by an editor, not an author                  |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| key-points        | autre             |  An abstract which lists the key points made by the article       |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| objetives         | autre             |  An abstract used for Learning Objectives or article objectives   |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| section           | autre             |  An abstract containing the titles of an article’s sections;      |
|                   |                   |  following each title, that section is summarized.                |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| stereochemical    | autre             |  An abstract containing only the details of a chemical compound,  |
|                   |                   |  for example, one major publisher’s “stereochem” abstract         |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| teaser            | autre             |  A short abstract specifically written to create interest in the  |
|                   |                   |  reader                                                           |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| web-summary       | autre             |  Short summary intended for distribution on a website             |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| other             | autre             |  Refers to books. It can also represent only a part or chapter of |
|                   |                   |  a book.                                                          |
+-------------------+-------------------+-------------------------------------------------------------------+
| toc               | chapeau           |  A very short abstract, usually only a line or two long, that is  |
|                   |                   |  displayed in a Table of Contents                                 |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| short             | abrege            |  An abbreviated form of the abstract, for example, for use inside |
|                   |                   |  a generated Table of Contents, or to be returned in addition to  |
|                   |                   |  the article title during a search                                |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+
| summary           | resume            |  Summation of the article, typically used in conjunction with     |
|                   |                   |  other types of abstracts                                         |
|                   |                   |                                                                   |
+-------------------+-------------------+-------------------------------------------------------------------+