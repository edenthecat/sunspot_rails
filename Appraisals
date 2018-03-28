ruby_version = Gem::Version.new(RUBY_VERSION)

if ruby_version < Gem::Version.new('2.2.0')
  ['3.0.0', '3.1.0'].each do |rails_version|
    appraise "rails-#{rails_version}" do
      gem 'sunspot', path: File.expand_path('sunspot', ENV['SUNSPOT_LIB_HOME'])
      gem 'sunspot_solr', path: File.expand_path('sunspot_solr', ENV['SUNSPOT_LIB_HOME'])
      gem 'rails', "~> #{rails_version}"
      gem 'progress_bar', '~> 1.0.5', require: false
      gem 'rspec', '~> 3.4.0'
      gem 'rspec-rails', '~> 3.4.0'
    end
  end
end

if ruby_version < Gem::Version.new('2.4.0')
  appraise 'rails-3.2.0' do
    gem 'sunspot', path: File.expand_path('sunspot', ENV['SUNSPOT_LIB_HOME'])
    gem 'sunspot_solr', path: File.expand_path('sunspot_solr', ENV['SUNSPOT_LIB_HOME'])
    gem 'rails', '~> 3.2.0'
    gem 'progress_bar', '~> 1.0.5', require: false
    gem 'test-unit', '~> 3.2.0'
    gem 'rspec', '~> 3.4.0'
    gem 'rspec-rails', '~> 3.4.0'
  end

  ['4.0.0', '4.1.0'].each do |rails_version|
    appraise "rails-#{rails_version}" do
      gem 'sunspot', path: File.expand_path('sunspot', ENV['SUNSPOT_LIB_HOME'])
      gem 'sunspot_solr', path: File.expand_path('sunspot_solr', ENV['SUNSPOT_LIB_HOME'])
      gem 'rails', "~> #{rails_version}"
      gem 'protected_attributes'
      gem 'progress_bar', '~> 1.0.5', require: false
      gem 'rspec', '~> 3.4.0'
      gem 'rspec-rails', '~> 3.4.0'
    end
  end
end

appraise 'rails-4.2.0' do
  gem 'sunspot', path: File.expand_path('sunspot', ENV['SUNSPOT_LIB_HOME'])
  gem 'sunspot_solr', path: File.expand_path('sunspot_solr', ENV['SUNSPOT_LIB_HOME'])
  gem 'rails', '~> 4.2.0'
  gem 'protected_attributes'
  gem 'progress_bar', '~> 1.0.5', require: false
  gem 'rspec', '~> 3.4.0'
  gem 'rspec-rails', '~> 3.4.0'
end

if ruby_version >= Gem::Version.new('2.2.0')
  ['5.0.0', '5.1.0'].each do |rails_version|
    appraise "rails-#{rails_version}" do
      gem 'sunspot', path: File.expand_path('sunspot', ENV['SUNSPOT_LIB_HOME'])
      gem 'sunspot_solr', path: File.expand_path('sunspot_solr', ENV['SUNSPOT_LIB_HOME'])
      gem 'rails', "~> #{rails_version}"
      gem 'protected_attributes_continued'
      gem 'progress_bar', '~> 1.0.5', require: false
    end
  end
end
