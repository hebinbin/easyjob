easyjob
=======

# assume one month is 30 days, one year is 360days

def compare(y1, m1, d1, y2, m2, d2)
  result = (y1 - y2)*360 + (m1 - m2)*30 + (d1 - d2)
  if result.abs == 30
    p "1 month apart"
  elsif result.abs > 30
    p "greater than 1 month apart"
  else 
    p "lesser than 1 month apart"  
  end  
end

compare(2002, 1, 28, 2001, 12, 28)
