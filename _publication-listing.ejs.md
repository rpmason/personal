<% for (const item of items) { %>
::: {.publication-item}
### <%= item.title %>

[<%= item.authors %>]{.publication-authors}

[<%= item.venue %><% if (item.year) { %>, <%= item.year %><% } %>]{.publication-venue}
<% if (item.note) { %>
[<%- item.note %>]{.publication-note}
<% } %><% if (item.links) { %>
[<% for (const link of item.links) { %>[<%= link.text %>](<%= link.href %>) <% } %>]{.publication-links}
<% } %>
:::
<% } %>
