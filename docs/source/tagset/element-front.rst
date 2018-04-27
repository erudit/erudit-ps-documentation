.. _element-front:

<front>
=======

+-------------------------+------------+
| Appears in              | Frequency  |
+=========================+============+
| :ref:`element-article`  | Once       |
+-------------------------+------------+


The initial set of metadata of the document, usually called as *front metadata*.

Elements found in ``<front>``:

+------------------------------+
| Tags                         |
+==============================+
| :ref:`element-journal-meta`  |
+------------------------------+
| :ref:`element-article-meta`  |
+------------------------------+

Example:

.. code-block:: xml

  ...
  <front>
    <journal-meta>
      <journal-id journal-id-type="publisher-id">rum</journal-id>
      <journal-title-group>
        <journal-title>Revue de l'Université de Moncton</journal-title>
      </journal-title-group>
      <issn pub-type="epub">1712-2139</issn>
      <issn pub-type="ppub">0316-6368</issn>
      <publisher>
        <publisher-name>Revue de l'Université de Moncton</publisher-name>
      </publisher>
    </journal-meta>
    <article-meta>
      <title-group>
        <article-title>De la préservation linguistique et nationale : la qualité de la langue de la jeunesse acadienne, un débat linguistique idéologique</article-title>
      </title-group>
      <contrib-group>
        <contrib>
          <name>
            <surname>Arrighi</surname>
            <given-names>Laurence</given-names>
          </name>
          <xref ref-type="aff" rid="aff1"/>
        </contrib>
        <contrib>
          <name>
            <surname>Violette</surname>
            <given-names>Isabelle</given-names>
          </name>
          <xref ref-type="aff" rid="aff1"/>
        </contrib>
      </contrib-group>
      <aff id="aff1">
        <institution content-type="orgname">Université de Moncton</institution>
      </aff>
      <pub-date date-type="pub">
        <year>2013</year>
      </pub-date>
      <volume>44</volume>
      <issue>2</issue>
      <fpage>67</fpage>
      <lpage>101</lpage>
      <abstract>
        <p>Cet article a pour objectif d’analyser un débat linguistique idéologique centré sur le rapport établi entre l’avenir de la francophonie canadienne, la qualité de la langue et le devoir de la jeunesse en la matière. L’idée que la jeunesse serait particulièrement responsable de la dégradation de la langue fait l’objet d’un discours ancien et sans cesse redéployé. Nous proposons une approche critique de son actualisation récente en Acadie, telle qu’elle s’est manifestée dans des publications médiatiques aux parentés argumentatives fortes, entre l’automne 2012 et le printemps 2013. Afin d’objectiver les prises de position, nous montrons qu’elles puisent légitimité et autorité dans les fondements idéologiques du nationalisme politique moderne, qui font de la langue le ciment de l’identité collective et de sa « bonne maîtrise » une compétence accessible sur base démocratique.</p>
      </abstract>
      <trans-abstract xml:lang="en">
        <p>This article analyses the language ideological debate surrounding the relationship between the future of the Canadian Francophonie, the quality of the language, and the duty of young people to preserve it. The idea that young people in particular are responsible for the deterioration of a language is part of an old and recurring discourse. We examine its resurgence between the fall of 2012 and the spring of 2013 in Acadie, as seen in media texts that share strong argumentative similarities. Through a critical approach, we show that the positions staked out in this debate draw their legitimacy and authority from the ideological foundations of modern political nationalism, which construe language as the central feature of identity and language proficiency as a skill that is accessible to all.</p>
      </trans-abstract>
      <kwd-group xml:lang="fr">
        <kwd>francophonie minoritaire canadienne</kwd>
        <kwd>qualité de la langue</kwd>
        <kwd>jeunesse</kwd>
        <kwd>nationalisme linguistique</kwd>
        <kwd>idéologie linguistique</kwd>
      </kwd-group>
      <kwd-group xml:lang="es">
        <kwd>Canadian Francophone minority</kwd>
        <kwd>language quality</kwd>
        <kwd>youth</kwd>
        <kwd>linguistic nationalism</kwd>
        <kwd>language ideology</kwd>
      </kwd-group>
    </article-meta>
  </front>
  ...

.. {"reviewed_on": "201804627", "by": "fabio.batalha@erudit.org"}
