# Test
{
StrToMember(
    "[period].[period].[" +
    [}ElementAttributes_period].(
        StrToMember(
            "[period].[period].[" +
            NumberToString(Val(Subst([period].[period].[202607QTD].Name, 1, 6)) - 100) + "QTD]"
        ),
        [base_period]
    ) + "]"
)
}
