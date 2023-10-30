<script>
	import Nav from "../../components/Nav.svelte";
    import dataStatic from "../../data/dataStatic";

</script>
<div class="font-jetbrains-mono flex justify-center mx-[5%]">
	<div class="w-[500px] mt-10 flex flex-col gap-8">
        <Nav />
        <h1 class="text-lg font-semibold text-center">Contacts</h1>
        <ul>
            <li>{dataStatic.contacts.email}</li>
            <li><a href={dataStatic.contacts.linkedin}>@rahman-muhaemin</a></li>
            <li>{dataStatic.contacts.github}</li>
            <li>{dataStatic.contacts.telegram}</li>
            <li>{dataStatic.contacts.website}</li>
        </ul>
    </div>
</div>
