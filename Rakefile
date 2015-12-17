namespace :generate do
  ROOT = File.expand_path('..', __FILE__)
  PLANTUML_JAR = File.join(ROOT, 'vendor/plantuml.jar')

  def plantuml(files)
    `java -jar #{PLANTUML_JAR} #{files.join(' ')}`
  end

  task :sequence do
    plantuml(Dir[File.join(ROOT, 'doc/**/*.seq')])
  end
end
