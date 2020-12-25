# parameter
```
module param_list
(
parameter width = 128;
parameter height = 64;
input [width-1:0]  a;
input [height-1:0] b;
......
)
endmodule
```

## Before the instance
``` param_list #(256, 128) u0 (.a(a), .b(b));```

## inside the instance
``` param_list #(.width(128), .height(128)) u0(.a(a), .b(b));```

## use defparam
```
param_list u0(.a(a), .b(b));
defparam u0.width = 256;
```
# generate
