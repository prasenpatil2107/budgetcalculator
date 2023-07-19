<script>
    let columns = ['Heading 1','Heading 2','Heading 4','Heading 5','add'];
    let values=[
        {1:'test1',2:'test2',4:'test4',5:'test5',6:"<button>ttest</button>"},
        {1:'test1',2:'test2',4:'test4',5:'test5',6:"<button>ttest</button>"},
    ]
  </script >

<body>
    <table>
      <thead>
        <tr>
            {#each columns as columnHeading}
              <th>{columnHeading}</th>
            {/each}
          <tr/>
        {#each Object.values(values) as row}
            <tr>
            {#each Object.values(row) as cell}
                <td>{cell}</td>
            {/each}
            </tr>
        {/each}
      </thead>
      <tbody>
        <tr>
          <td></td>
        </tr>
      </tbody>
    </table>
  </body>   
  <style>
    table, th, td {
      border: 1px solid;
      border-collapse: collapse;
      margin: 10px;
    }
  </style>
  