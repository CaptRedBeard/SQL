# SQL
Some useful code

--Gives Fiscal Year adjust 1 & 6 to suit actual months that fall in the Fiscal Year
case when month(cast([Posted Month] as varchar)) between 1 and 6 then year(cast([Posted Month] as varchar))
								else year(cast(a.[Pymt Posted Month] as varchar)) + 1 end
