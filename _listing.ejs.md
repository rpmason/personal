<% for (const item of items) { %>
::: {.post-listing-item}
### [<%= item.title %>](<%= item.path %>)

<%- item.description %>

[Date: <%= item.date %> | Author: Richard Mason]{.post-meta-line}
:::
<% } %>
