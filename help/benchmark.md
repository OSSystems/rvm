Benchmark

If you have a bit of code that you would like to benchmark, across several versions of ruby all at once, you can now do this easily with RVM. Given:

  ∴ cat increment.rb
    y=0
    1000.times do |x|
      y = x + 1
    end
We can benchmark this code against multiple ruby versions very easily:

  ∴ rvm 1.8.6,1.8.7,1.9.1,ree benchmark increment.rb


Documentation:

https://rvm.io/set/benchmark/
