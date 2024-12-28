# Tables

Display structured data in a tabular format.

## Basic Table

| Header 1 | Header 2 | Header 3 |
|----------|----------|----------|
| Cell 1   | Cell 2   | Cell 3   |
| Cell 4   | Cell 5   | Cell 6   |

## Styled Table

<div class="table-container">
  <table class="styled-table">
    <thead>
      <tr>
        <th>Feature</th>
        <th>Description</th>
        <th>Status</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Responsive</td>
        <td>Adapts to screen size</td>
        <td><Badge type="tip" text="Active" /></td>
      </tr>
      <tr>
        <td>Sortable</td>
        <td>Click headers to sort</td>
        <td><Badge type="warning" text="Beta" /></td>
      </tr>
    </tbody>
  </table>
</div>

<style>
.table-container {
  overflow-x: auto;
  margin: 2rem 0;
}

.styled-table {
  width: 100%;
  border-collapse: collapse;
  background: white;
  border-radius: 0.5rem;
  overflow: hidden;
  box-shadow: 0 1px 3px rgba(0, 0, 0, 0.1);
}

.styled-table th,
.styled-table td {
  padding: 1rem;
  text-align: left;
  border-bottom: 1px solid #e5e7eb;
}

.styled-table thead {
  background: #f9fafb;
}

.styled-table tbody tr:hover {
  background: #f3f4f6;
}
</style>