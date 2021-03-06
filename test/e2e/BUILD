package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_test(
    name = "go_default_test",
    srcs = [
        "e2e_test.go",
        "metrics_grabber_test.go",
        "taints_test.go",
    ],
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = [
        "//pkg/client/clientset_generated/clientset:go_default_library",
        "//test/e2e/api:go_default_library",
        "//test/e2e/autoscaling:go_default_library",
        "//test/e2e/cluster-logging:go_default_library",
        "//test/e2e/extension:go_default_library",
        "//test/e2e/framework:go_default_library",
        "//test/e2e/metrics:go_default_library",
        "//test/e2e/scalability:go_default_library",
        "//test/e2e/scheduling:go_default_library",
        "//test/e2e/storage:go_default_library",
        "//test/e2e/workload:go_default_library",
        "//test/utils:go_default_library",
        "//vendor/github.com/onsi/ginkgo:go_default_library",
        "//vendor/github.com/onsi/gomega:go_default_library",
        "//vendor/github.com/stretchr/testify/assert:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/fields:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//vendor/k8s.io/client-go/tools/cache:go_default_library",
    ],
)

go_library(
    name = "go_default_library",
    srcs = [
        "addon_update.go",
        "apparmor.go",
        "audit.go",
        "cadvisor.go",
        "certificates.go",
        "cluster_upgrade.go",
        "custom_resource_definition.go",
        "dashboard.go",
        "disruption.go",
        "dns.go",
        "dns_common.go",
        "dns_configmap.go",
        "e2e.go",
        "empty_dir_wrapper.go",
        "etcd_failure.go",
        "events.go",
        "example_cluster_dns.go",
        "examples.go",
        "firewall.go",
        "garbage_collector.go",
        "generated_clientset.go",
        "gke_local_ssd.go",
        "gke_node_pools.go",
        "ha_master.go",
        "ingress.go",
        "kibana_logging.go",
        "kube_proxy.go",
        "kubectl.go",
        "kubelet.go",
        "kubelet_perf.go",
        "limit_range.go",
        "logging_soak.go",
        "monitoring.go",
        "namespace.go",
        "network_partition.go",
        "network_policy.go",
        "networking.go",
        "networking_perf.go",
        "no-snat.go",
        "nodeoutofdisk.go",
        "nvidia-gpus.go",
        "pod_gc.go",
        "podpreset.go",
        "pods.go",
        "portforward.go",
        "pre_stop.go",
        "proxy.go",
        "reboot.go",
        "resize_nodes.go",
        "resource_quota.go",
        "restart.go",
        "security_context.go",
        "service.go",
        "service_accounts.go",
        "service_latency.go",
        "serviceloadbalancers.go",
        "ssh.go",
        "stackdriver_monitoring.go",
        "ubernetes_lite.go",
        "util_iperf.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/api/v1/pod:go_default_library",
        "//pkg/api/v1/service:go_default_library",
        "//pkg/apis/batch/v2alpha1:go_default_library",
        "//pkg/apis/networking:go_default_library",
        "//pkg/client/clientset_generated/clientset:go_default_library",
        "//pkg/client/clientset_generated/clientset/typed/certificates/v1beta1:go_default_library",
        "//pkg/client/clientset_generated/internalclientset:go_default_library",
        "//pkg/cloudprovider:go_default_library",
        "//pkg/cloudprovider/providers/azure:go_default_library",
        "//pkg/cloudprovider/providers/gce:go_default_library",
        "//pkg/controller:go_default_library",
        "//pkg/controller/endpoint:go_default_library",
        "//pkg/controller/node:go_default_library",
        "//pkg/kubectl/cmd/util:go_default_library",
        "//pkg/kubelet/apis:go_default_library",
        "//pkg/kubelet/apis/stats/v1alpha1:go_default_library",
        "//pkg/kubelet/pod:go_default_library",
        "//pkg/master/ports:go_default_library",
        "//pkg/quota/evaluator/core:go_default_library",
        "//pkg/util/exec:go_default_library",
        "//pkg/util/logs:go_default_library",
        "//pkg/util/version:go_default_library",
        "//plugin/pkg/admission/serviceaccount:go_default_library",
        "//test/e2e/chaosmonkey:go_default_library",
        "//test/e2e/common:go_default_library",
        "//test/e2e/framework:go_default_library",
        "//test/e2e/framework/ginkgowrapper:go_default_library",
        "//test/e2e/generated:go_default_library",
        "//test/e2e/manifest:go_default_library",
        "//test/e2e/metrics:go_default_library",
        "//test/e2e/scheduling:go_default_library",
        "//test/e2e/upgrades:go_default_library",
        "//test/e2e/workload:go_default_library",
        "//test/e2e_federation:go_default_library",
        "//test/images/net/nat:go_default_library",
        "//test/utils:go_default_library",
        "//test/utils/junit:go_default_library",
        "//vendor/github.com/elazarl/goproxy:go_default_library",
        "//vendor/github.com/ghodss/yaml:go_default_library",
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/google/cadvisor/info/v1:go_default_library",
        "//vendor/github.com/influxdata/influxdb/client/v2:go_default_library",
        "//vendor/github.com/onsi/ginkgo:go_default_library",
        "//vendor/github.com/onsi/ginkgo/config:go_default_library",
        "//vendor/github.com/onsi/ginkgo/reporters:go_default_library",
        "//vendor/github.com/onsi/gomega:go_default_library",
        "//vendor/golang.org/x/crypto/ssh:go_default_library",
        "//vendor/golang.org/x/net/websocket:go_default_library",
        "//vendor/golang.org/x/oauth2/google:go_default_library",
        "//vendor/google.golang.org/api/monitoring/v3:go_default_library",
        "//vendor/k8s.io/api/batch/v1:go_default_library",
        "//vendor/k8s.io/api/batch/v2alpha1:go_default_library",
        "//vendor/k8s.io/api/certificates/v1beta1:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/api/extensions/v1beta1:go_default_library",
        "//vendor/k8s.io/api/policy/v1beta1:go_default_library",
        "//vendor/k8s.io/api/rbac/v1beta1:go_default_library",
        "//vendor/k8s.io/api/settings/v1alpha1:go_default_library",
        "//vendor/k8s.io/apiextensions-apiserver/pkg/apis/apiextensions/v1beta1:go_default_library",
        "//vendor/k8s.io/apiextensions-apiserver/pkg/client/clientset/clientset:go_default_library",
        "//vendor/k8s.io/apiextensions-apiserver/test/integration/testserver:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/fields:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/intstr:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/net:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/uuid:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/yaml:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/serviceaccount:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/registry/generic/registry:go_default_library",
        "//vendor/k8s.io/client-go/discovery:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/client-go/rest:go_default_library",
        "//vendor/k8s.io/client-go/tools/cache:go_default_library",
        "//vendor/k8s.io/client-go/util/cert:go_default_library",
        "//vendor/k8s.io/client-go/util/flowcontrol:go_default_library",
    ],
)

genrule(
    name = "gen_e2e.test",
    testonly = 1,
    srcs = [":go_default_test"],
    outs = ["e2e.test"],
    cmd = "srcs=($(SRCS)); cp $$(dirname $${srcs[0]})/go_default_test $@;",
    output_to_bindir = 1,
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//test/e2e/api:all-srcs",
        "//test/e2e/autoscaling:all-srcs",
        "//test/e2e/chaosmonkey:all-srcs",
        "//test/e2e/cluster-logging:all-srcs",
        "//test/e2e/common:all-srcs",
        "//test/e2e/extension:all-srcs",
        "//test/e2e/framework:all-srcs",
        "//test/e2e/generated:all-srcs",
        "//test/e2e/manifest:all-srcs",
        "//test/e2e/metrics:all-srcs",
        "//test/e2e/perftype:all-srcs",
        "//test/e2e/scalability:all-srcs",
        "//test/e2e/scheduling:all-srcs",
        "//test/e2e/storage:all-srcs",
        "//test/e2e/testing-manifests:all-srcs",
        "//test/e2e/upgrades:all-srcs",
        "//test/e2e/workload:all-srcs",
    ],
    tags = ["automanaged"],
)
