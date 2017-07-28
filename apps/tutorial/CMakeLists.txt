foreach (exec_file BFS BellmanFord Components Radii KCore)
    add_executable(tutorial_${exec_file} ${exec_file}.C)
    target_include_directories(tutorial_${exec_file} PUBLIC "../../ligra")
endforeach ()

add_executable(tutorial_encoder ../../ligra/encoder.C)
target_include_directories(tutorial_encoder PUBLIC "../../ligra")
