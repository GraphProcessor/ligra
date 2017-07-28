foreach (exec_file ACL-Serial ACL-Serial-Naive ACL-Serial-Opt ACL-Serial-Opt-Naive HeatKernel-Serial HeatKernel-Randomized-Serial Nibble-Serial)
    add_executable(${exec_file} ${exec_file}.C)
    target_include_directories(${exec_file} PUBLIC "../../ligra")
endforeach ()

foreach(para_exec_file ACL-Sync-Local ACL-Sync-Local-Opt HeatKernel-Parallel HeatKernel-Randomized-Parallel Nibble-Parallel)
    add_executable(${para_exec_file} ${para_exec_file}.C)
    target_include_directories(${para_exec_file} PUBLIC "../../ligra")
endforeach ()