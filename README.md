# assignment-3

CREATE FUNCTION MultiplyByTwo(@Value INT)
RETURNS INT
AS
BEGIN
    RETURN @Value * 2
END;

CREATE FUNCTION MultiplyByFour(@Value INT)
RETURNS INT
AS
BEGIN
    RETURN dbo.MultiplyByTwo(@Value) * 2
END;
