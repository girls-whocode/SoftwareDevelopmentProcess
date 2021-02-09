# BSL

usage: **\`\`\`bsl**

renders:

```bsl
# Domain Name Area

Remes A Export;

# If Server then

// Comment procedure
&On server
Procedure Name Procedure (
    Values ​​of Parameter Constant,
    NormalParameter,
    Parameter with an Incorrect Value = Illegal,
    Parameter with Incorrect Value = NelegalNo Space,
    Parameter with Default Numbers Value = 0) Export
    a =? (NOT ValueCompleted (Undefined), "", "Is value";
    B = "text with screened" "quotation mark" + "and concatenations" "";

    B = "multiline
    | string
    // | this is a comment
    | // but this is not
    | ";
    G = "";

    TextRequest = TextRequest +? (TextRequest = "", "
        | CHOOSE ","
        | COMBINE ALL
        | CHOOSE ") +"
        | Date, Link, Submission, Held, Mark Deletion,
        ""?
        ""?
        ""?
        | FROM Document. "+ KeyNumber.Key +"
        | WHERE Link In (& "+ KeyNumber.Key +") ";

    TextRequest =
        "CHOOSE
        | Table.Field AS Field,
        | MAXIMUM (Table.Field2) AS Field2
        | FROM
        | Table AS Table
        | WHERE
        | Table.Field = 0
        | And Table. In the field <> "" String "" "+" 123 "+"
        | AND EXPRESS (Table. In the field LIKE A LINE) <> "" ""
        | And Table. Field <> "" string with screened "" "" quotation mark ""
        // | Commented line
        | // Commented string inside the query with quotation marks "" TEXT ""
        | COUNT BY
        | Field
        | // AUTO ORDERING ";

    GUID = 00000000-0000-0000-0000-000000000000;
    Number = 0.0 * 100;
    NumberFrom = Number ("1000");

    Date = '00010101000000';
    ShortDate = '00010101';
    Data Splitting = '0001-01-01';

    If A = 0 AND NOT Number <= 0 Then
        NormalParameter = True;
    Otherwise
        NormalParameter = False;
    End If;
    Bye ValueFilled (B) Cycle
        Interrupt;
    End of the Cycle;

    Unstructured Procedure ();

    NewObject = New Value Table;
    NewObject = New ("Table of Values");

    PrefixValue FilledPostfix = "";

EndProcedure

Non-Built Procedure ()
    Return;
EndProcedure

#End If

# End Area
```
