def product(a)
    prod = 1
    i = 0
    while (i<a.size)
      prod = prod*a[i]
      i=i+1
    end
    puts "#{prod}"
    end
    
    product([234, 121, 23, 945, 0])

    -----------------------------------------------------------------------

    def anagrams?(firstw, secondw)

    _firstw = firstw.chars.sort
    _secondw = secondw.chars.sort

    anagrams = _firstw == _secondw

    puts "#{anagrams}"
    end

    anagrams?('paT', 'Tap')

    -----------------------------------------------------------------------------


    def compare(firstw, secondw)
  
      compare = firstw.chars == secondw.chars
  
      puts "#{compare}"
      end
  
      compare('GoOd DaY', 'gOOd dAy')

---------------------------------------------------------------------------------

def key_in_hash hash
  hash.keys.map(&:to_s).sort_by do |item|
    item.length
  end
end

puts key_in_hash({ abc: 'hello', another_key: 123, 4567 => 'third' })

----------------------------------------------------------------------------------

'When you call super without any parameters, Ruby sends a message to the parent of 
the current object, asking it to call a method with the same name as the method from which
you called super and the parameters passed to the method. On the other hand, when called
with super(), it does not send any parameters to the parent.'
