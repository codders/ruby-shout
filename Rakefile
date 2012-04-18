require 'rubygems'
require 'rubygems/package_task'

spec = Gem::Specification.new {|s|
    s.name = 'ruby-shout'
    s.version = '2.1.1'
    s.author = 'Jared Jennings'
    s.email = 'jjenning@fastmail.fm'
    s.homepage = 'http://www.dingoskidneys.com/~jaredj/'
    s.platform = Gem::Platform::RUBY
    s.summary = 'Send audio over the network to an Icecast server'
    s.files = ['ext/shout.c', 'ext/extconf.rb', 'example.rb']
    s.has_rdoc = true
    s.extra_rdoc_files = ['README']
    s.extensions = ['ext/extconf.rb']
    s.autorequire = 'shout'
    s.require_path = '.'
}

Gem::PackageTask.new(spec) do |pkg|
  pkg.gem_spec = spec
  pkg.need_tar = true
end

