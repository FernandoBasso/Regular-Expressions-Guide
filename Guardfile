require 'asciidoctor'

guard 'shell' do
  watch(/(README|docs\/.+)\.adoc$|.+\.ts$/) do |m|
    Asciidoctor.convert_file('./README.adoc', :safe => :unsafe)
    print "\n\nChanged #{m[0]}\n\n"
  end
end

# guard 'shell' do
#   watch(/(^.+\/)?.*\.adoc$/) do |m|
#     Asciidoctor.convert_file(m[0], :safe => :unsafe)
#     n m[0], 'File Changed'
#     # `say -v changed #{m[0]}`
#   end
# end

#
# vim: set ft=ruby:
#
