foreach (exec_file BFS BC BellmanFord Components Radii PageRank PageRankDelta BFSCC BFS-Bitvector KCore MIS Triangle CF)
    add_executable(${exec_file} ${exec_file}.C)
    target_include_directories(${exec_file} PUBLIC "../../ligra")
endforeach ()

