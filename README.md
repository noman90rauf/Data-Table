Data-Table
==========

DataTables Editor v1.3.3 library with data table multiselect and input type file options

If you ant to add input type "file" in data table form simply add this dataTables.editor.min.js and following code:

  $(document).ready(function () {
    editor = new $.fn.dataTable.Editor({
        table: "#example",
        fields: [ {
                label: "Icon:",
                name: "file",
                id: "upload",
                type: "file" // Using the custom field type
              }
        ],
        ajax: path + "groups/createGroup"
    });
  });
  
  Too add multiselect add following code:
  
  $(document).ready(function () {
    editor = new $.fn.dataTable.Editor({
        table: "#example",
        fields: [ {
                label: "Icon:",
                name: "file",
                id: "upload",
                type: "file" // Using the custom field type
              }, {
                label: "Members:",
                name: "members",
                type: "select",
                multiple: "true",
                ipOpts: getStudent()
            }
        ],
        ajax: path + "groups/createGroup"
    });
  });
  
  For more detail email me:
  
  noman90rauf@gmail.com
  
  
  
