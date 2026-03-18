task :build do
  require 'erubi/capture_block'
  File.open("public/index.html", "wb") do |f|
    f << eval(Erubi::CaptureBlockEngine.new(File.read('index.html.erb')).src)
  end
end
