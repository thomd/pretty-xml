#
# generate gemspec file
#
# rake -T 
#
begin
  require 'jeweler'
  Jeweler::Tasks.new do |gemspec|
    gemspec.name = "pretty-xml"
    gemspec.version = "0.2.0"
    gemspec.summary = "Pretty print XML."
    gemspec.description = "Pretty print XML depends upon Nokogiri to perform XML transformation."
    gemspec.homepage = "http://github.com/thomd/pretty-xml/"
    gemspec.add_dependency "nokogiri", ">= 1.4.1"
  end
  Jeweler::GemcutterTasks.new
rescue LoadError
  puts "Jeweler not available. Install it with: gem install jeweler"
end
