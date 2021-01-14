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

If you want to create a new PDf file from the current v1.6. markdown file, call the following command in the MarkDown dir(requires font DejaVuSans):

"pandoc --pdf-engine=xelatex -V geometry:"top=2cm,bottom=1.5cm,left=2cm,right=2cm" -V mainfont:"DejaVuSans" -V monofont:"DejaVuSans" SAMM-1.6.md -f markdown-implicit_figures -o SAMM_Core_V1-6_FINAL.pdf"

This command requires \\pagebreak and \\newpage commands in the markdown file (which are currently included)

## SAMM 1.6 Markdown Changelog v1.6

* Images
  * changed image locations to its own directory 'images/', changed links
  * changed image descriptions
  * deleted '#' from image links
  * changed the following images in order to integrate all 16 security practices in v1.6
    * Cover (v1.5 -> v1.6)
    * SAMM-Overview (4 new security practices)
    * PNGDoc (deleted)
* License
  * linting
* Executive Summary
  * linting
  * added indentation
* Contents
  * linting
  * set new page numbers
  * facilitated the format

* Understanding the model
  * deleted '#'
  * Business Functions
    * 'twelve' -> 'sixteen'
    * set new page numbers
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
  * in all Business Functions / Security Practices:
    * tables rearranged for better latex-based conversion to PDF
    * linting and alignment
  * Security Culture added
  * Security Design added
  * Security Pentesting added
  * Security Monitoring added

* Security Practices in detail (linting in all sec practice && levels && escaping '>')
  * *all*:
    * linting sec practices && levels
    * escaping '>'
    * changing table format so that it is correctly displayed in github (5 columns -> 4 columns)
    * changed ordering of "Related Levels" to match the SAMM-overview order
  * SM
    * SM1
    * deleted '.' in activity summary sentence
    * SM2
      * results -> ##### Results
  * PC
  * EG
    * EG1: Results, deleted new line
  * added Sec Culture
  * TA
    * TA2: deleted star in related levels section
  * SR
    * SR1
      * objective ###Consider -> ### Consider
  * SA
  * added Sec Design
  * DR
    * DR3
      * Related Levels: "Code Review" -> "Implementation Review"
  * IR
    * IR1-3 added space: 'Implementation Review:IR1' -> 'Implementation Review: IR1
  * ST
  * added Sec Pentesting
  * IM
    * IM2
      * third party -> third-party
  * EH
    * Table: Results EH3: two stars --> one star ("Reinforced operational environment...")
  * OE
  * added Sec Monitoring

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
