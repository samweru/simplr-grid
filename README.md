Simplr Grid
===========
![simplrGrid](https://raw.githubusercontent.com/samweru/simplr-grid/master/img/simplrGrid-min.png)

## Usage

```js

$("#data-grid").simplrGrid({

    url:"/server/fetch.all.php",
    method:"POST",
    title:"Sample Grid",
    usePager:true,
    // data:jsonData, //use when inserting data directly
    singleSelect:true,
    columnHide:[

        // "id"
    ],
    toolbars:[

        //[btnAdd, btnSel] //create and insert elements into multiple toolbars directly
    ],
    css:{

        width:500,
        height:500
    },
    pager:{

        page:1,
        rows:10//,
        // list:[10,20]
    },
    onDblClick:function(row){//row double click event

        console.log(row);
    }
})
.fixLeftColumn()
.fixHeader()
.resizeColumns();
```

## Plugins

`simplrGrid` - is a plugin by itself but also includes other plugins that are already used in grid functionality. If you so wish to use them individually on other elements, you may do so but with some adjustment to your code.

1. `resizeColumns` - use header to resize columns
2. `fixHeader` - fix header row
3. `fixLeftColumn` - fix left most column
4. `getSelected` - gets single or first `tr.selected` (returns json)
5. `getAllSelected` - gets multiple `tr.selected` (returns json list)

## Contributions

Thanks a lot to the developer(s) of the plugin(s) below: 

[TableHeadFixer](https://github.com/lai32290/TableHeadFixer)

Have fun!
