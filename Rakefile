require 'html/proofer'
require 'yaml'

task :test do
  sh "bundle exec jekyll build"
  HTML::Proofer.new("./_site", check_html: true).run
end
