foreach (exec_file rMatGraph gridGraph randLocalGraph SNAPtoAdj adjGraphAddWeights adjToBinary)
add_executable(${exec_file} ${exec_file}.C)
target_include_directories(${exec_file} PUBLIC "../ligra")
endforeach ()
