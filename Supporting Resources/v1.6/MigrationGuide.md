# SAMM 1.5 to 1.6 Migration Guide

## General Considerations

Most importantly, we added one new security practice for each business function.
The background was that we missed some points in securing the Software Lifecycle.
The new security practices are called:

* Security Culture, part of governance
* Security Design, part of construction
* Security Pentesting. part of verification
* Security Monitoring, part of operations

Please refer to the markdown or PDF file for further information.

We also managed to "bug-fix" the assessment toolbox files of v1.5.
Please refer to the following sections for detailed information.

If you want to inspect the markdown file with a linter, prefer the markdownlinter extension of VS code.
Use the available .markdownlint.json config file and add the following exceptions:
{
    "MD001" : false,
    "MD013" : false,
    "MD024" : false,
    "MD036" : false,
    "MD041" : false
}

## SAMM 1.6 Markdown Changelog v1.6

* Images
  * changed image locations to its own directory 'images/', changed links
  * deleted '#' from image links
  * changed the following images in order to integrate all 16 security practices in v1.6
    * Cover (v1.5 -> v1.6)
    * SAMM-Overview (4 new security practices)
    * PNGDoc (deleted)
* License
  * linting
* Executive Summary
  * linting
* Contents
  * linting
  * TODO set new page numbers

* Understanding the model
  * deleted '#'
  * Business Functions
    * 'twelve' -> 'sixteen'
    * TODO set new page numbers >
    * Governance
      * added Security Culture + linting all
    * Construction
      * changed "Construction:" to "Construction"
      * added Security Design + linting all
    * Verification
      * added Security Pentesting + linting all
    * Operations
      * added Security Monitoring + linting all
    * Maturity Levels
      * None
  
* Governance (linting)
  * Description & Activity overview & Assessment worksheet
    * SM, PC, EG: linting and alignment
    * Security Culture added
* Construction (linting)
  * Description & Activity overview & Assessment worksheet
    * TA, SR, SA: linting and alignment
    * Security Design added
* Verification (linting) and alignment
  * Description & Activity overview & Assessment worksheet
    * DR, IP, ST: linting and alignment
    * Security Pentesting added
* Operations (linting)
  * Description & Activity overview & Assessment worksheet
    * IM, EH, OE: linting and alignment
    * Security Monitoring added

* Security Practices in detail (linting in all sec practice && levels && escaping '>')
  * *all*:
    * linting sec practices && levels
    * escaping '>'
    * changing table format so that it is correctly displayed in github (5 columns -> 4 columns)
  * SM
    * SM1
    * deleted '.' in activity summary sentence
    * SM2
      * results -> ##### Results
  * PC
  * EG
    * EG1: Results, deleted new line
  * Sec Culture
  * TA
  * SR
    * SR1
      * objective ###Consider -> ### Consider
  * SA
  * Sec Design
  * DR
  * IR
    * IR1-3 added space: 'Implementation Review:IR1' -> 'Implementation Review: IR1
  * ST
  * Sec Pentesting
  * IM
    * IM2
      * third party -> third-party
  * EH
  * OE

## SAMM Assessment Toolbox Changelog v1.6

* Attribution and License
  * added author
  * changed version to v1.6

* Interview
  * 4 new Security Practices with at least 2 guidances in each level
  * guidance SA3,1 changed broken cell format

* Scorecard
  * added new security practices
  * fixed reference that falsely showed the exact same diagram for phase 2-4
  * simplified references in column U
  * fixed alignment
  * some minor design improvements (borders)
  * "business functions" vs. "functions" only --> functions only
  * column width and row height fixes

* Roadmap
  * added new security practices
  * changed bordering format (current state)

* Roadmap Chart
  * added new security practices

* Lookups
  * added security practice level references
  * corrected some (but not all(sic!)) old level references (e.g. G-Table, construction, 18, G->C)

## OWASP Books Instructions

* changed version & file name
* improved content via linter
* small spelling corrections
