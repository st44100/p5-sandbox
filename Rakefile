task :default => ["run"]

task :run do
  sketch_path = File.dirname(__FILE__)
  output_path = sketch_path + "/build" 
  sh "processing-java --run --sketch=#{sketch_path} --output=#{output_path} --force"
end

task :mvim do
  sh 'osascript -e "tell application \"MacVim\"" -e "activate" -e "end tell"'
end

task :back do
  sh "osascript -e 'tell application \"System Events\"' -e 'keystroke tab using {command down}' -e 'end tell'"
end
