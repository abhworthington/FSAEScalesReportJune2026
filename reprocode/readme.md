## Readme for Reproducability Files

These files are the source for the website seen at <https://www.abhworthington.com/FSAEScalesReportJune2026/FSAEJ2026Report.html>. The site is compiled in Quarto, using a combination of YAML, Markdown, and R. The workflow for this project is:
- data collection and entry into an Excel workbook, containing
  - Car list
  - Design Times
  - Corner weights (driver in) and car only weight (driver out) entered as lb, converted to kg
  - Vehicle characteristics (either copied from Google Forms output or entered manually from paper sheets)
  - Miscellaneous calculations for sticker creation
- within workbook, transfer of necessary data to an "export sheet"
- R imports sheet from Excel, creates source dataframe for tables and viz
- Within Quarto Chunks, tables and viz created in R, knitted with Markdown to create HTML page (the site)

Additionally, a PDF for printing and offline reading was produced, similar code with small edits and format difference for pandoc. See comparison of headers.
