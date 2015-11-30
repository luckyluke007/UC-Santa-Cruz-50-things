require 'html/proofer'

# rake test
desc "Build and test the site"
task :test do
  sh "bundle exec jekyll build"
   HTML::Proofer.new("./build", {:verbose => true, :disable_external => true}).run
  sh "bundle exec scss-lint"
end