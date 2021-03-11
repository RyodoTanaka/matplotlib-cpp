cmake_minimum_required(VERSION 2.8.3)

set(SOURCES
  animation
  basic
  fill
  imshow
  minimal
  nonblock
  subplot2grid
  surface
  xkcd
  bar
  colorbar
  fill_inbetween
  lines3d
  modern
  quiver
  subplot
  update
  )

foreach(src ${SOURCES})
  add_executable(${src} ${src}.cpp)
  target_link_libraries(${src} ${PYTHON_LIBRARIES})
endforeach()




