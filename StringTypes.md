Markdown | Less | Pretty
char(n) | Fixed width character string | 8,000 characters | Defined width
varchar(n) | Variable width character string | 8,000 characters | 2 bytes + number of chars
varchar(max) | Variable width character string | 1,073,741,824 characters | 2 bytes + number of chars
text | Variable width character string | 2GB of text data | 4 bytes + number of chars
nchar | Fixed width Unicode string | 4,000 characters | Defined width x 2
nvarchar | Variable width Unicode string | 4,000 characters	 
nvarchar(max) | Variable width Unicode string | 536,870,912 characters	 
ntext | Variable width Unicode string | 2GB of text data	 
binary(n) | Fixed width binary string | 8,000 bytes	 
varbinary | Variable width binary string | 8,000 bytes	 
varbinary(max) | Variable width binary string | 2GB	 
image | Variable width binary string | 2GB

Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the 
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
