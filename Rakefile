namespace :greeting do
  desc 'outputs hello to the terminal'
    task :hello do
      puts 'hello from Rake!'
    end

  desc 'outputs hola to the terminal'
    task :hola do
      puts 'hola de Rake!'
    end
  end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

  desc 'some description'
  task :environment do
    require_relative './config/environment.rb'
  end

  desc 'seed database with dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end

end



#   namespace :db
#     db:migrate
#       invokes the :environment task as a dependency (FAILED - 3)
#       create the students table in the database (FAILED - 4)
#     db:seed
#       seeds the database with dummy data from a seed file (FAILED - 5)
