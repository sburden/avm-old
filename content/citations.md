# Citations

To include citations:

1. Modify the file in `_bibliography/references.bib`.  
2. In your content, add the following text to include a citation
   
   ```
   {% raw %}{% cite bibtex_cite_key %}{% endraw %}
   ```
   For example, the text `{% raw %}{% cite Perge2012-vm %}{% endraw %}` generates the citation {% cite Perge2012-vm %}.

   You can also include multiple citations in one go --  `{% raw %}{% cite Perge2012-vm MacKay1952-om %}{% endraw %}` generates {% cite Perge2012-vm MacKay1952-om %}.

3. Generate a bibliography on your page using the following text:

   ``` 
   {% raw %}{% bibliography %}{% endraw %}
   ```

   This will generate a bibliography for your entire BibTeX file; to list only the citations that appear on the current page, use the following syntax:

   ```
   {% raw %}{% bibliography --cited %}{% endraw %}
   ```

# References cited

{% bibliography --cited %}

# All references 

{% bibliography %}

