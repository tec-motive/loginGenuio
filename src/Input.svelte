<script>
  export let icon;
  export let type;
  // export let placeholder
  // 플레이스 홀더는 추가 준비 중

</script>

<div class="relative">
  <i class="{icon} absolute z-10 left-4 top-4 text-gray-300"></i>
  <input class="m-2 w-60 p-1 relative" type={type}>
</div>
